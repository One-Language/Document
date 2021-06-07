1. [Manage One](/core-manage-One): install `One` **and** add `One` to your shell
2. [Manage Plugins](/core-manage-plugins): add a plugin for your tool `One plugin add nodejs`
3. [Manage Versions](/core-manage-versions): install a version of that tool `One install nodejs 13.14.0`
4. [Configuration](/core-configuration): set global and project tool versions via `.tool-versions` config

## Install

### Dependencies

<!-- select:start -->
<!-- select-menu-labels: Operating System,Installation Method -->

#### -- Linux,Aptitude --

```shell
sudo apt install curl git
```

#### -- Linux,DNF --

```shell
sudo dnf install curl git
```

#### -- Linux,Pacman --

```shell
sudo pacman -S curl git
```

#### -- Linux,Zypper --

```shell
sudo zypper install curl git
```

#### -- macOS,Homebrew --

Dependencies will be automatically installed by Homebrew.

#### -- macOS,Spack --

```shell
spack install coreutils curl git
```

### -- Docsify Select Default --

No match for _Operating System_ and _Installation Method_ selections. Please try another combination.

<!-- select:end -->

### One

<!-- select:start -->
<!-- select-menu-labels: Installation Method -->

### --Git--

Clone only the latest branch:

```shell
git clone https://github.com/One-Language/One.git ~/.One --branch v0.8.1
```

Alternately, you can clone the whole repo and checkout the latest branch:

```shell
git clone https://github.com/One-Language/One.git ~/.One
cd ~/.One
git checkout "$(git describe --abbrev=0 --tags)"
```

### --Homebrew--

!> See `One` and Homebrew compatibility [issues in #785](https://github.com/One-Language/One/issues/785) before continuing.

Install using the Homebrew package manager:

```shell
brew install One
```

To use the latest changes, you can point Homebrew to the master branch of the repo:

```shell
brew install One --HEAD
```

### --Pacman--

Install using `pacman`:

```shell
git clone https://aur.archlinux.org/One-vm.git
cd One-vm
makepkg -si
```

Or use your preferred [AUR helper](https://wiki.archlinux.org/index.php/AUR_helpers)

<!-- select:end -->

### Add to your Shell

<!-- select:start -->
<!-- select-menu-labels: Operating System,Shell,Installation Method -->

#### --Linux,Bash,Git--

Add the following to `~/.bashrc`:

```shell
. $HOME/.One/One.sh
```

?> Completions must be configured by adding the following to your `.bashrc`:

```shell
. $HOME/.One/completions/One.bash
```

#### --Linux,Fish,Git--

Add the following to `~/.config/fish/config.fish`:

```shell
source ~/.One/One.fish
```

?> Completions must be configured manually with the following command:

```shell
mkdir -p ~/.config/fish/completions; and ln -s ~/.One/completions/One.fish ~/.config/fish/completions
```

#### --Linux,ZSH,Git--

Add the following to `~/.zshrc`:

```shell
. $HOME/.One/One.sh
```

**OR** use a ZSH Framework plugin like [One for oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/One) which will source this script and setup completions.

?> Completions are configured by either a ZSH Framework `One` plugin or by adding the following to your `.zshrc`:

```shell
# append completions to fpath
fpath=(${One_DIR}/completions $fpath)
# initialise completions with ZSH's compinit
autoload -Uz compinit
compinit
```

- if you are using a custom `compinit` setup, ensure `compinit` is below your sourcing of `One.sh`
- if you are using a custom `compinit` setup with a ZSH Framework, ensure `compinit` is below your sourcing of the framework

!> if you are using a ZSH Framework the associated `One` plugin may need to be updated to use the new ZSH completions properly via `fpath`. The Oh-My-ZSH One plugin is yet to be updated, see <https://github.com/ohmyzsh/ohmyzsh/pull/8837>.

#### --Linux,Bash,Pacman--

Add the following to `~/.bashrc`:

```shell
. /opt/One-vm/One.sh
```

?> [`bash-completion` needs to be installed for the completions to work](https://wiki.archlinux.org/title/bash#Common_programs_and_options)

#### --Linux,Fish,Pacman--

Add the following to `~/.config/fish/config.fish`:

```shell
source /opt/One-vm/One.sh
```

!> Completions are automatically configured on installation by the AUR package.

#### --Linux,ZSH,Pacman--

Add the following to `~/.zshrc`:

```shell
. /opt/One-vm/One.sh
```

?> Completions are placed in a ZSH friendly location, but [ZSH must be configured to use the autocompletions](https://wiki.archlinux.org/index.php/zsh#Command_completion).

#### --macOS,Bash,Git--

If using **macOS Catalina or newer**, the default shell has changed to **ZSH**. Unless changing back to Bash, follow the ZSH instructions.

Add the following to `~/.bash_profile`:

```shell
. $HOME/.One/One.sh
```

?> Completions must be configured manually with the following entry in your `.bash_profile`:

```shell
. $HOME/.One/completions/One.bash
```

#### --macOS,Fish,Git--

Add the following to `~/.config/fish/config.fish`:

```shell
source ~/.One/One.fish
```

?> Completions must be configured manually with the following command:

```shell
mkdir -p ~/.config/fish/completions; and cp ~/.One/completions/One.fish ~/.config/fish/completions
```

#### --macOS,ZSH,Git--

Add the following to `~/.zshrc`:

```shell
. $HOME/.One/One.sh
```

**OR** use a ZSH Framework plugin like [One for oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/One) which will source this script and setup completions.

?> Completions are configured by either a ZSH Framework `One` plugin or by adding the following to your `.zshrc`:

```shell
# append completions to fpath
fpath=(${One_DIR}/completions $fpath)
# initialise completions with ZSH's compinit
autoload -Uz compinit
compinit
```

- if you are using a custom `compinit` setup, ensure `compinit` is below your sourcing of `One.sh`
- if you are using a custom `compinit` setup with a ZSH Framework, ensure `compinit` is below your sourcing of the framework

!> if you are using a ZSH Framework the associated `One` plugin may need to be updated to use the new ZSH completions properly via `fpath`. The Oh-My-ZSH One plugin is yet to be updated, see <https://github.com/ohmyzsh/ohmyzsh/pull/8837>.

#### --macOS,Bash,Homebrew--

If using **macOS Catalina or newer**, the default shell has changed to **ZSH**. Unless changing back to Bash, follow the ZSH instructions.

Add `One.sh` to your `~/.bash_profile` with:

```shell
echo -e "\n. $(brew --prefix One)/One.sh" >> ~/.bash_profile
```

?> Completions will need to be [configured as per Homebrew's instructions](https://docs.brew.sh/Shell-Completion#configuring-completions-in-bash) or with the following:

```shell
echo -e "\n. $(brew --prefix One)/etc/bash_completion.d/One.bash" >> ~/.bash_profile
```

#### --macOS,Fish,Homebrew--

Add `One.fish` to your `~/.config/fish/config.fish` with:

```shell
echo -e "\nsource "(brew --prefix One)"/One.fish" >> ~/.config/fish/config.fish
```

?> Completions are [handled by Homebrew for the Fish shell](https://docs.brew.sh/Shell-Completion#configuring-completions-in-fish). Friendly!

#### --macOS,ZSH,Homebrew--

Add `One.sh` to your `~/.zshrc` with:

```shell
echo -e "\n. $(brew --prefix One)/One.sh" >> ${ZDOTDIR:-~}/.zshrc
```

**OR** use a ZSH Framework plugin like [One for oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/One) which will source this script and setup completions.

?> Completions are configured by either a ZSH Framework `One` or will need to be [configured as per Homebrew's instructions](https://docs.brew.sh/Shell-Completion#configuring-completions-in-zsh). If you are using a ZSH Framework the associated One plugin may need to be updated to use the new ZSH completions properly via fpath. The Oh-My-ZSH One plugin is yet to be updated, see [ohmyzsh/ohmyzsh#8837](https://github.com/ohmyzsh/ohmyzsh/pull/8837).

### --Docsify Select Default--

!> The `Homebrew` `One` Formulae has not been tested on `Linux` by the core One team. Please raise an issue if this has changed and we will update the docs.

<!-- select:end -->

Restart your shell so that PATH changes take effect. (Opening a new terminal
tab will usually do it.)

You are ready to use One 🎉

### Having Issues?

If you're having issues with your shell not detecting newly installed shims, it's most-likely due to the sourcing of `One.sh` or `One.fish` not being at the **BOTTOM** of your `.bash_profile`, `.zshrc`, `config.fish` config file. It needs to be sourced **AFTER** you have set your `$PATH` and **AFTER** you have sourced your framework (oh-my-zsh etc).

### Migrating Tools

If you're migrating from other tools and want to use your existing version files (eg: `.node-version` or `.ruby-version`), look at the `legacy_version_file` [flag in the configuration section](core-configuration?id=homeOnerc).

## Update

<!-- select:start -->
<!-- select-menu-labels: Installation Method -->

### -- Git --

```shell
One update
```

If you want the latest changes that aren't yet included in a stable release:

```shell
One update --head
```

### -- Homebrew --

```shell
brew upgrade One
```

### -- Pacman --

Manually download a new `PKGBUILD` and rebuild or use your preferred AUR helper.

<!-- select:end -->

## Remove

To uninstall `One` follow these steps:

<!-- select:start -->
<!-- select-menu-labels: Operating System,Shell,Installation Method -->

### --Linux,Bash,Git--

1. In your `~/.bashrc` remove the lines that source `One.sh` and the completions:

```shell
. $HOME/.One/One.sh
. $HOME/.One/completions/One.bash
```

2. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --Linux,Fish,Git--

1. In your `~/.config/fish/config.fish` remove the lines that source `One.sh`:

```shell
source ~/.One/One.fish
```

and remove completions with this command:

```shell
rm -rf ~/.config/fish/completions/One.fish
```

2. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --Linux,ZSH,Git--

1. In your `~/.zshrc` remove the lines that source `One.sh` and completions:

```shell
. $HOME/.One/One.sh
# ...
fpath=(${One_DIR}/completions $fpath)
autoload -Uz compinit
compinit
```

**OR** the ZSH Framework plugin if used.

2. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --Linux,Bash,Pacman--

1. In your `~/.bashrc` remove the lines that source `One.sh` and the completions:

```shell
. /opt/One-vm/One.sh
```

2. Uninstall with your package manager:

```shell
pacman -Rs One-vm
```

3. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

4. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --Linux,Fish,Pacman--

1. In your `~/.config/fish/config.fish` remove the lines that source `One.fish`:

```shell
source /opt/One-vm/One.fish
```

2. Uninstall with your package manager:

```shell
pacman -Rs One-vm
```

3. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

4. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --Linux,ZSH,Pacman--

1. In your `~/.zshrc` remove the lines that source `One.sh`:

```shell
. /opt/One-vm/One.sh
```

2. Uninstall with your package manager:

```shell
pacman -Rs One-vm
```

3. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

4. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --macOS,Bash,Git--

1. In your `~/.bash_profile` remove the lines that source `One.sh` and the completions:

```shell
. $HOME/.One/One.sh
. $HOME/.One/completions/One.bash
```

2. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --macOS,Fish,Git--

1. In your `~/.config/fish/config.fish` remove the lines that source `One.fish`:

```shell
source ~/.One/One.fish
```

and remove completions with this command:

```shell
rm -rf ~/.config/fish/completions/One.fish
```

2. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --macOS,ZSH,Git--

1. In your `~/.zshrc` remove the lines that source `One.sh` and completions:

```shell
. $HOME/.One/One.sh
# ...
fpath=(${One_DIR}/completions $fpath)
autoload -Uz compinit
compinit
```

**OR** the ZSH Framework plugin if used.

2. Remove the `$HOME/.One` dir:

```shell
rm -rf ${One_DATA_DIR:-$HOME/.One}
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --macOS,Bash,Homebrew--

If using **macOS Catalina or newer**, the default shell has changed to **ZSH**. If you can't find any config in your `~/.bash_profile` it may be in a `~/.zshrc` in which case please follow the ZSH instructions.

1. In your `~/.bash_profile` remove the lines that source `One.sh` and the completions:

```shell
. $(brew --prefix One)/One.sh
. $(brew --prefix One)/etc/bash_completion.d/One.bash
```

?> Completions may have been [configured as per Homebrew's instructions](https://docs.brew.sh/Shell-Completion#configuring-completions-in-bash) so follow their guide to find out what to remove.

2. Uninstall with your package manager:

```shell
brew uninstall One --force
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --macOS,Fish,Homebrew--

1. In your `~/.config/fish/config.fish` remove the lines that source `One.fish`:

```shell
source "(brew --prefix One)"/One.fish
```

2. Uninstall with your package manager:

```shell
brew uninstall One --force
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

### --macOS,ZSH,Homebrew--

1. In your `~/.zshrc` remove the lines that source `One.sh`:

```shell
. $(brew --prefix One)/One.sh
```

2. Uninstall with your package manager:

```shell
brew uninstall One --force
```

3. Run this command to remove all `One` config files:

```shell
rm -rf $HOME/.tool-versions $HOME/.Onerc
```

<!-- select:end -->

That's it! 🎉
