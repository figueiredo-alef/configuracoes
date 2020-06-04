# Instalação do Oh My ZSH

* Instale o Curl:
  ```
  $ sudo apt install curl
  ```
* Instale o ZSH:
  ```
  $ sudo apt install zsh
  ```
* Instale o OhMyZSH:
  ```
  $ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  ```
**OBs:** Durante a instalação do Oh My ZSH será questionado se você deseja alterar o seu shell padrão para o ZSH, basta digitar “Y” e pressionar “Enter”. Digite sua senha em seguida e pressione "Enter".

* Instale o SPACESHIP:
  ```
  $ git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"
  
  $ ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
  ```
* Execute o comando abaixo para abrir o arquivo oculto .zshrc:
  ```
  $ code ~/.zshrc
  ```
  * Ao abrir altere a variável que contém o nome do tema para ZSH_THEME="spaceship" e salve o arquivo.

* Reinicie a Sessão (sem fechar o Terminal).
* Abra novamente o arquivo .zshrc e adicione a configuração abaixo:
  ```
  SPACESHIP_PROMPT_ORDER=(
    user
    dir
    host
    git
    exec_time
    line_sep
    vi_mode
    jobs
    exit_code
    char
  )

  SPACESHIP_PROMPT_ADD_NEWLINE=false
  SPACESHIP_CHAR_SYMBOL="❯"
  SPACESHIP_CHAR_SUFFIX=" "
  ```
* Salve o arquivo. Reinicie o Terminal.

* Instale o zinit:
  ```
  $ sh -c "$(curl -fsSL https://raw.githubusercontent.com/zdharma/zinit/master/doc/install.sh)"
  ```
  
* Digite "y" e pressione "Enter".

  
* Insira as configurações abaixo no arquivo .zshrc:
  ```
  zinit light zsh-users/zsh-autosuggestions
  zinit light zsh-users/zsh-completions
  zinit light zdharma/fast-syntax-highlighting
  ```

  * Salve o arquivo.

* Para mostrar o virtualenv no terminal insira as configurações abaixo no arquivo .zshrc:
  ```
  # Show virtualenv
  export VIRTUAL_ENV_DISABLE_PROMPT=
  ```

  * Salve o arquivo e reinicie a Sessão.

---

[**Início**](https://github.com/figueiredo-alef/configuracoes/blob/master/README.md) | [**Anterior**](https://github.com/figueiredo-alef/configuracoes/blob/master/outros-programas.md) | [**Próximo**](https://github.com/figueiredo-alef/configuracoes/blob/master/pycharm.md)

---

Feito por [Alef Figueiredo](https://github.com/figueiredo-alef)
