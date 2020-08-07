# ohmyzh

Configuração de terminal do Oh Myzh

# Instalação

Primeiro instale o zsh e o oh-my-zsh:

```shell
$ sudo dnf install zsh -y
$ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
$ sudo chsh -s /bin/zsh root
```

Em seguida, instale o tema:

```shell
$ git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"
$ ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```

Instale os plugins:

```shell
$ git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

Aplique as configurações:

```shell
$ git clone https://github.com/gustavoleitao/ohmyzh.git
$ mv ~/.zshrc ~/.zshrc-bkp
$ cp ohmyzh/.zshrc ~/.zshrc
```
