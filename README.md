# Mac Development Ansible Playbook

This repository is a fork of Jeff Geerlings excellent repository: https://github.com/geerlingguy/mac-dev-playbook
It is a stripped version suited to my needs.

For installation:
 
``` xcode-select --install
    sudo easy_install pip
    sudo pip install ansible
    cd /tmp/
    git clone git@github.com:f1gjam/mac-dev-playbook.git
    cd /tmp/mac-dev-playbook
    ansible-galaxy install -r requirements.yml
```
```
    #For Ansible >= 2.0 use
    ansible-playbook -i inventory --ask-become-pass main.yml
```

The dot files will be pulled down from the dot files repo.

**Note**: Some dot file are created from scratch within the ansible tasks.
