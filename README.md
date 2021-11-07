# 

```bash
sudo apt install zsh
```

```bash
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
git clone https://github.com/rulweb/zsh-rulweb ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-rulweb
```

```bash
git clone git@github.com:rulweb/srv.dotfiles.git ~/.dotfiles
rm ~/.zshrc
ln -s ~/.dotfiles/.aliases ~/.aliases
ln -s ~/.dotfiles/.zshrc ~/.zshrc
```
