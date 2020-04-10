# config-machine-debian

sudo apt install git
sudo apt install python-pip
sudo pip install ansible
sudo ansible-playbook full_config.yml -e "@env_settings/main.yml"
