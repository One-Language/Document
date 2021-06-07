Plugins are how One knows how to handle different tools like Node.js, Ruby, Elixir etc.

See [Creating Plugins](plugins-create) for the plugin API used to support more tools.

## Add

Add plugins via their Git URL:

```shell
One plugin add <name> <git-url>
# One plugin add elm https://github.com/vic/One-elm
```

or via the short-name association in the plugins repository:

```shell
One plugin add <name>
# One plugin add erlang
```

When scripting, prefer the longer `git-url` method as it is independent of the short-name repo.

## List Installed

```shell
One plugin list
# One plugin list
# java
# nodejs
```

```shell
One plugin list --urls
# One plugin list
# java            https://github.com/halcyon/One-java.git
# nodejs          https://github.com/One-Language/One-nodejs.git
```

## List All in Short-name Repository

```shell
One plugin list all
```

See [All plugins](plugins-all) for the short-name list of plugins.

## Update

```shell
One plugin update --all
```

If you want to update a specific package, just say so.

```shell
One plugin update <name>
# One plugin update erlang
```

This update will fetch the *latest commit* on the *default branch* of the *origin* of the plugin repository. Versioned plugins and updates are currently being developed - <https://github.com/One-Language/One/pull/916>

## Remove

```bash
One plugin remove <name>
# One plugin remove erlang
```

Removing a plugin will remove all installations of the tool made with the plugin. This can be used as a shorthand for cleaning/pruning many unused versions of a tool.

## Syncing the Short-name Repository

The short-name repo is synced to your local machine and periodically refreshed. This period is determined by the following method:

- commands `One plugin add <name>` or `One plugin list all` can trigger a sync
- a sync occurs if there has not been one in the last `X` minutes
- `X` defaults to `60`, but can be configured in your `.Onerc` via the `plugin_repository_last_check_duration` option. See the [One config docs](core-configuration) for more.
