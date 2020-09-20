# Vim

## 1. Install

neovim 설치
```bash
brew install neovim

# MesloLGS NF가 없는 경우
brew tap caskroom/fonts
brew cask install font-meslolg-nerd-font
```

apply neovim

```bash
$ vim ~/.zshrc

alias vim="nvim"
alias vi="nvim"
alias vimdiff="nvim -d"
export EDITOR=/usr/local/bin/nvim

$ source ~/.zshrc
```

## 2. Plugins

install SpaceVim

```bash
curl -sLf https://spacevim.org/install.sh | bash
```

## 3. Vim Themes

```bash
mkdir ~/.SpaceVim.d/colors
curl https://gist.githubusercontent.com/subicura/91696d2da58ad28b5e8b2877193015e1/raw/6fb5928c9bda2040b3c9561d1e928231dbcc9184/snazzy-custom.vim -o ~/.SpaceVim.d/colors/snazzy-custom.vim

$ vim ~/.SpaceVim.d/init.toml
```

## Reference

- [본격 macOS에 개발 환경 구축하기](https://subicura.com/2017/11/22/mac-os-development-environment-setup.html#system-preferences)