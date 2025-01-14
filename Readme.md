# dotfiles

## Prerequisits

### direnv

set up your shell with direnv : https://github.com/direnv/direnv/blob/master/docs/hook.md
```
brew install direnv
```

### Tuckr : https://github.com/RaphGL/Tuckr

Super powered replacement for GNU Stow. Tuckr uses RustCrypto's chacha20poly1305 as it's encryption cipher and so we can even save secrets with this tool.

Install from rust cargo 
```
cargo install --git https://github.com/RaphGL/Tuckr.git
```

## Install This repo

Install dotfiles
```
git clone git@github.com:manu4linux/tuckr-files.git ~/.dotfiles
```

Edit .envrc and .gitconfig to your username ssh and run direnv
```
cd ~/.dotfiles
cat .envrc 
direnv allow .
```

## Flow of operations 

- Auto run's `direnv` which invoke variables based on file `.envrc`.

### Add dotfile links to its place 

 Manually run Tuckr add \<group> : `tuckr add zsh` to set dotfiles
    - run `tuckr add \<group>` is we need hooks scripts to run

### remove dotfile links to its place 

- tuckr status
- tuckr rm \<group> : `tuckr rm zsh`


## TODO

- nix based setup 
- golang with asdf
- rust with ??
- dart with ??
