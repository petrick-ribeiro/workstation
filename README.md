# Workstation

## :robot: Automating Workstation Setup with Ansible.

> A Playbook to prepare and pre-configure a fresh install of Ubuntu >= 18.xx distribution version.

### Getting Started

#### Prereqs:
``` shell
sudo apt-get update && sudo apt-get install python3-pip
python3 -m pip install --user ansible
```
> In case the Ansible directory is not on **PATH** use **export PATH="$HOME/.local/bin:$PATH"**

#### Clone the repo:
```shell
git clone https://github.com/petrick-ribeiro/workstation.git &&\
cd workstation
```

#### Run the playbook:
```shell
ansible-playbook setup.yml --ask-become-pass
```
> This playbook is geared towards improve DevOps workflow.

#### Setup Starship prompt
```shell
ansible-playbook starship.yml --ask-become-pass
```
> Before run this playbook reload your shell session.
