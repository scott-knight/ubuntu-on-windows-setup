# Customize Ubuntu

This document explains how to customize Ubuntu. This document assumes you have followed the installation and setup instrcutions from all of the previous steps.  

<br/>

## Update Ubuntu

1. Close all open `Windows Terminal` windows. Open a new `Ubuntu` window. 
2. You should update `Ubuntu` with the latest security patches and other default updates by running the following:

```sh
sudo bash -c 'for i in update {,dist-}upgrade auto{remove,clean}; do apt-get $i -y; done'
```

<br/>

## Install Wajig and Keychain

`Wajig` is a simple package installation tool. `Keychain` Allows you to store your `SSH` keys in a local keychain for the time your Windows OS is up and running. To install the utilities, run the following:

```sh
sudo apt-get install wajig keychain
```

Once finished, run the following:

```sh
wajig update
```

You will use this command to update Ubuntu from now on. 

<br/>

## Install Build-Essential and Related Utilities

To install `build-essential` and related utilities, run the following:

```sh
wajig install -y build-essential pkg-config libssl-dev
```

<br/>

Setup for these files will come in a later step.

<br/>

## Install Git

To install Git, run the following:

```sh
wajig install -y git
```

<br/>

## Install Zsh

To install zsh, run the following:

```sh
wajig install -y zsh 
```

To make zsh your default shell, run the following:

```sh
chsh -s $(which zsh)
```

Once changed, close the terminal instance and open a new Ubuntu instance.

You will be prompted to make a selection to create a `.zshrc` file. Select the option that simply adds the comment code and creates the file.

Close all instances and start a new Ubuntu instance.

<br/>

## Create System Files

Run the following:

```sh
touch .zsh_functions .zsh_alias_list .pryrc .gemrc .gitconfig
```
<br/>

## Install RBENV and BREW Depenencies

Install the required utilities by running the following:

```sh
wajig install -y gcc clang make libssl-dev libreadline-dev zlib1g-dev
```

<br/>

## Install BREW for Linux

Reference found [here](https://docs.brew.sh/Homebrew-on-Linux)

1. To install BREW for Linux, run the following:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. You should be prompted about default settings and installation. Simply accept the defaults.
3. Once finished, add the following to your `.zshrc` file

> eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"

4. Reload the ubuntu shell.
5. Add BREW taps

```sh
brew tap Homebrew/homebrew-cask && brew tap Homebrew/homebrew-services && brew tap homebrew/cask-versions && brew tap Homebrew/homebrew-core
```

6. Install a basic set of utilities

```sh
brew install automake curl-openssl elixir erlang node@14 postgres python ruby sqlite
```

<br/>

## INSTALL RBENV

To install RBENV, run the following:

```sh
git clone https://github.com/rbenv/rbenv.git ${HOME}/.rbenv
```

Add the following to `.zshrc`:

> # RBENV
> export RBENV_ROOT="${HOME}/.rbenv"
> export PATH="${RBENV_ROOT}/bin:${RBENV_ROOT}/shims:$PATH"
> if which rbenv > /dev/null; then eval "$(rbenv init - zsh)"; fi
 
Close and reload the Ubuntu instance

<br/>

## Install ruby-build rbenv-gemset rbenv-whatis rbenv-use

To install RBENV plugins, run the following:





