# Terminal

## 1. Install Iterm2

```bash
$ brew install iterm2 --cask
```

## 2. Zsh

Mac OS default가 zsh로 변경되어 따로 zsh을 설치할 필요는 없다.

### **ohmyzsh**

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

https://github.com/ohmyzsh/ohmyzsh

### **zsh plugins**

- zsh-syntax-highlighting

명령어 하이라이팅 플러그인

```bash
$ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

https://github.com/zsh-users/zsh-syntax-highlighting

- zsh-autosuggestions

명령어 자동완성 플러그인

```bash
$ git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

https://github.com/zsh-users/zsh-autosuggestions

- fzf

히스토리 검색(^ + R) 및 다양한 기능 제공

```bash
$ brew install fzf
```

### **apply plugins**

```bash
$ vim ~/.zshrc

plugins=(
  git
  fzf
  zsh-syntax-highlighting
  zsh-autosuggestions
)
```

### **zsh themes**

- Powerlevel10k

```bash
$ git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k
```

```bash
$ p10k configure
```

apply theme

```bash
$ vim ~/.zshrc

ZSH_THEME="powerlevel10k/powerlevel10k"
```

### **zsh insecure completion issue**

```bash
$ vim ~/.zshrc

ZSH_DISABLE_COMPFIX=true
```
