# Installation

Need to ensure that the operating environment meets the following requirements:

* PHP >= 7.1
* Swoole PHP extension >= 4.4
* PDO PHP extension （If you need to use MySQL Client）
* Redis PHP extension （If you need to use Redis Client）

## Create project via Composer

```bash
composer create-project simple-swoole/skeleton
```

!> If you need to use `MySQL` and` Redis` clients, and `Swoole` version is less than` v4.4.17`, you need to install [Swoole/Library](https://github.com/swoole/library) , At the same time, you need to add `-d swoole.enable_library = off` or modify `php.ini` to close the built-in `library` at startup

```bash
composer require swoole/library:dev-master
```

## Start

Support HTTP Server, WebSocket Server and MQTT Server.

```bash
php bin/simps.php http:start
php bin/simps.php ws:start
php bin/simps.php mqtt:start
```

The Server configuration file is in `config/servers.php`.

## Custom Server

For example, if you need a separate TCP service, you need to encapsulate it yourself and add the relevant information in the configuration file.

```php
return [
    // Other parts omitted.
    'tcp' => [
        'ip' => '0.0.0.0',
        'port' => 9504,
        'sock_type' => SWOOLE_SOCK_TCP,
        'callbacks' => [
        ],
        'settings' => [
        ],
        // Setting up the startup server class
        'class_name' => \App\Server\TCP::class
    ],
];
```

Executing the following command will start the corresponding service.

```shell
php bin/simps.php tcp:start
```
