# hackweek-ansible

Floating elephants ansible script. This should hopefully save you some time. If not, RIP.

This guide assumes you have the following already installed: git, pip, ansible, brew

*** THIS IS CURRENTLY SUPPORTED FOR MAC OSX ONLY ***

Settings before running:

- Please add your ssh public key (`~/.ssh/id_rsa.pub` or equivalent - if you don't have this, please use `ssh-keygen` to generate a new public-private key pair) to authorized keys on your host (in most cases this is just your local machine). This is usually located in `~/.ssh/authorized_keys`. If this file does not exists, create it, and add your public key with `cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys`.

- Add your ssh public key to your phabricator account. 

- run `ssh -T git@phab.trifacta.com` and proceed so that phabricator is added to your ssh known hosts.

- Please add `127.0.0.1` (aka localhost) to your `/etc/ansible/hosts` file. If this file does not exist, create first.

- If you haven't already, enable remote login, System Preferences > Sharing, for the current user. 

- if you want to add hosts to allow remote installation, put in `/etc/ansible/hosts`

- if you haven't already, please install brew: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`


#### MIGHT NEED BREW INSTALL BEFOREHAND