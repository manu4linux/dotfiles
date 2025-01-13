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

## Flow of operations 

- Auto run's `direnv` which invoke variables based on file `.envrc`.
### Add dotile links to its place 
 Manually run Tuckr set \<group> : `tuckr set zsh` to set dotfiles
### remove dotile links to its place 
- tuckr status
- tuckr rm \<group> : `tuckr rm zsh`