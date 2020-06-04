# CONFIGURAÇÕES BÁSICAS

- Abra o Terminal e execute o comando para checar possíveis atualizações pós instalação:
  ```
  $ sudo apt update
  ```

- Execute o comando para instalar as atualizações:
  ```
  $ sudo apt upgrade
  ```

- Reinicie a Sessão.

- Abra Configurações:
  - Desative o Bluetooth;
  - Na seção Som:
    - Aumente o volume de Sons do Sistema;
    - Altere o Som de Alerta;
  - Na seção Energia:
    - Em Apagar Tela selecione NUNCA;
    - Desative a Suspensão Automática;
    - Em Ação do Botão de Energia selecione SUSPENDER.
  - Na seção Monitores ative a Luz Noturna;
  - Na seção Mouse & Touchpad verifique se Rolagem Natural está desativada;
  - Na seção Usuários altere a Foto de Perfil.

- Pressione a tecla Super (ícone do Windows) e pesquise por Suporte a Idiomas. Será realizada uma busca por atualizações automaticamente. Reinicie a Sessão caso seja solicitado.

- Instalar a versão mais recente do Chrome requer [baixar o pacote .deb](https://www.google.com/intl/pt-BR/chrome/)

- Altere a versão padrão do Python:
  ```
  $ sudo ln -sf /usr/bin/python3.6 /usr/bin/python
  ```

- Instale o dconf Editor via Ubuntu Store.
  - Abra o programa e na Busca digite dash-to-dock;
  ```
    $ gsettings set org.gnome.shell.extensions.dash-to-dock click-action minimize-or-overview
    $ gsettings set org.gnome.shell.extensions.dash-to-dock dash-max-icon-size 34
    $ gsettings set org.gnome.shell.extensions.dash-to-dock dock-fixed false
    $ gsettings set org.gnome.shell.extensions.dash-to-dock dock-position BOTTOM
    $ gsettings set org.gnome.shell.extensions.dash-to-dock extend-height false
    $ gsettings set org.gnome.shell.extensions.dash-to-dock transparency-mode FIXED
    $ gsettings set org.gnome.shell.extensions.dash-to-dock unity-backlit-items true
    ```

---

[**Início**](https://github.com/figueiredo-alef/configuracoes/blob/master/README.md) | [**Próximo**](https://github.com/figueiredo-alef/configuracoes/blob/master/git-%26-ssh.md)

---

Feito por [Alef Figueiredo](https://github.com/figueiredo-alef)
