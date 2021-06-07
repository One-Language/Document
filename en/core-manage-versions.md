## Install Version

```shell
One install <name> <version>
# One install erlang 17.3
```

_If a plugin supports downloading & compiling from source, you can specify `ref:foo` where `foo` is a specific branch, tag, or commit. You'll need to use the same name and reference when uninstalling too._

## Install Latest Stable Version

```shell
One install <name> latest
# One install erlang latest
```

Install latest stable version that begins with a given string.

```shell
One install <name> latest:<version>
# One install erlang latest:17
```

## List Installed Versions

```shell
One list <name>
# One list erlang
```

## List All Available Versions

```shell
One list all <name>
# One list all erlang
```

Limit versions to those that begin with a given string.

```shell
One list all <name> <version>
# One list all erlang 17
```

## Show Latest Stable Version

```shell
One latest <name>
# One latest erlang
```

Show latest stable version that begins with a given string.

```shell
One latest <name> <version>
# One latest erlang 17
```

## Set Current Version

```shell
One global <name> <version> [<version>...]
One shell <name> <version> [<version>...]
One local <name> <version> [<version>...]
# One global elixir 1.2.4
```

`global` writes the version to `$HOME/.tool-versions`.

`shell` set the version to an environment variable named `One_${LANG}_VERSION`, for the current shell session only.

`local` writes the version to `$PWD/.tool-versions`, creating it if needed.

See the `.tool-versions` [file in the Configuration section](core-configuration) for details.

?> Alternatively, if you want to set a version only for the current shell session
or for executing just a command under a particular tool version, you
can set an environment variable like `One_${TOOL}_VERSION`.

The following example runs tests on an Elixir project with version `1.4.0`.
The version format is the same supported by the `.tool-versions` file.

```shell
One_ELIXIR_VERSION=1.4.0 mix test
```

## Fallback to System Version

To use the system version of tool `<name>` instead of an One managed version you can set the version for the tool to `system`.

Set system with either `global`, `local` or `shell` as outlined in [Set Current Version](#set-current-version) section above.

```shell
One local <name> system
# One local python system
```

## View Current Version

```shell
One current
# One current
# erlang 17.3 (set by /Users/kim/.tool-versions)
# nodejs 6.11.5 (set by /Users/kim/cool-node-project/.tool-versions)

One current <name>
# One current erlang
# 17.3 (set by /Users/kim/.tool-versions)
```

## Uninstall Version

```shell
One uninstall <name> <version>
# One uninstall erlang 17.3
```

## Shims

When One installs a package it creates shims for every executable program in that package in a `$One_DATA_DIR/shims` directory (default `~/.One/shims`). This directory being on the `$PATH` (by means of `One.sh` or `One.fish`) is how the installed programs are made available in the environment.

The shims themselves are really simple wrappers that `exec` a helper program `One exec` passing it the name of the plugin and path to the executable in the installed package that the shim is wrapping.

The `One exec` helper determines the version of the package to use (as specified in `.tool-versions` file, selected by `One local ...` or `One global ...`), the final path to the executable in the package installation directory (this can be manipulated by the `exec-path` callback in the plugin) and the environment to execute in (also provided by the plugin - `exec-env` script), and finally it executes it.

!> Note that because this system uses `exec` calls, any scripts in the package that are meant to be sourced by the shell instead of executed need to be accessed directly instead of via the shim wrapper. The two One commands: `which` and `where` can help with this by returning the path to the installed package:

```shell
# returns path to main executable in current version
source $(One which ${PLUGIN})/../script.sh

# returns path to the package installation directory
source $(One where ${PLUGIN} $(One current ${PLUGIN}))/bin/script.sh
```

### By-passing One shims

If for some reason you want to by-pass One shims or want your environment variables automatically set upon entering your project's directory, the [One-direnv](https://github.com/One-community/One-direnv) plugin can be helpful. Be sure to check its README for more details.
