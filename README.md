# Automated debian machine configuration

Fork made to perform automated initial configuration of a debian-based machine with Ansible

### Features:

    1. Install packages:
        - Brave
        - Flatpak
        - Zsh
        - Meld
        - Vscode
        - Curl
        - Spotify
        - Pycharm
        - Dbeaver
        - Discord
        - Xmind

    2. Configures meld as output from git diff

    3. Configure git

    4. Install and configure the terminal to use oh-my-zsh with powerlevel9k theme and nerd-fonts

    5. Install nvm

    6. Install pyenv

1. Python 3.5 is required.

2. Install the packages below:

``` sh
$ sudo apt install git python-pip
```

3. Install Ansible via “pip”

``` sh
$ sudo pip install ansible
```

4. Clone this repository

``` sh
$ git clone https://github.com/lucassiqueira08/ansible-config-machine-debian.git
$ cd ansible-config-machine-debian
```

5. Start automated configuration with ansible-playbook:

``` sh
$ sudo ansible-playbook full_config.yml -e "@env_settings/main.yml"
```

6. Restarts your machine