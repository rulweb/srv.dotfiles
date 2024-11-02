# 

```bash
sudo apt update && sudo apt install -y zsh
```

```bash
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Во время установки Oh My ZSH он спросит ставить ли его по умолчанию, конечно же ставим 😁

Скачиваем плагины для Oh My ZSH, я пользуюсь следующими:

• syntax-highlighting
• autosuggestions
• completions
• rulweb - мой плагин для автозаполнения Laravel Artisan и Composer команд, а так же сокращение php artisan до a и composer до c

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
git clone https://github.com/rulweb/zsh-rulweb ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-rulweb
```

И перечитываем конфигурации ZSH что бы изменения применились сразу, без перезапуска терминала

```bash
git clone https://github.com/rulweb/srv.dotfiles.git ~/.dotfiles
rm ~/.zshrc && ln -s ~/.dotfiles/.zshrc ~/.zshrc && ln -s ~/.dotfiles/.aliases ~/.aliases
source ~/.zshrc
```
