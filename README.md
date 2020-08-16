# Spin up Mac OS [Catalina] developer

👋 Hello friend!, This repo is a personal knowledge management and sharing system.

## Table of Contents

- Getting started
- Homebrew
- Git

- Powerline fonts
- Iterm
- Yarn
- NPM
- Typescript

By default macOs Catalina ships with a pre-installed git version.

Check the installed `git` version:

```git
git -v
```

## Homebrew

On macOS, the command to install Homebrew is:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

More: [A practical guide to Homebrew](https://flaviocopes.com/homebrew/)

## Homebrew and git ([Credit](https://stackoverflow.com/questions/8957862/how-to-upgrade-git-to-latest-version-on-macos/48953680#48953680))

In order to upgrade Git to latest version on macOS:

```bash
brew install git
```

Once it is installed, then type the following two lines, which will set our path to the local git distro instead of the Apple one.

```bash
export PATH=/usr/local/bin:$PATH
git --version
```

Symbolic link

```bash
brew link --force git
```

## Git

### Git useful commands

#### Git Revert

Note: Git revert in depth: [Link](https://stackoverflow.com/questions/4114095/how-do-i-revert-a-git-repository-to-a-previous-commit)

Reverting to a specific commit based on commit id with Git [Link](https://stackoverflow.com/questions/3639115/reverting-to-a-specific-commit-based-on-commit-id-with-git?lq=1)

```bash
git reset --hard <logid>
# example
git reset --hard 06a2331d1d1c750aec97788fe4b9a2e686298844
```

## Powerline fonts

Patched fonts for Powerline users, [Quick installation](https://github.com/powerline/fonts#quick-installation):

```bash
# clone
git clone https://github.com/powerline/fonts.git --depth=1
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts
```

## Iterm

Set bg to 10% Grey

## Yarn

```bash
brew install yarn
```

## NPM

Get list of globally installed packages:

```bash
npm list -g --depth 0
```

Uninstalling global packages:

```bash
npm uninstall -g <package_name>
```

## Typescript

Install typescript:

```bash
brew install typescript
```

## Terminal Commands

Clear command from terminal (clear/delete the current line):

```bash
CTRL+U
```
