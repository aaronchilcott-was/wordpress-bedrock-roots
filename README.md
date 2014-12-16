# Autopress

This will build a roots-bedrock vagrant instace with the roots scaffold theme.

## Requirements

1. Ansible >= 1.6 - [Installation docs](http://docs.ansible.com/intro_installation.html)
2. Virtualbox >= 4.3.10 - [Downloads](https://www.virtualbox.org/wiki/Downloads)
3. Vagrant >= 1.5.4 - [Downloads](http://www.vagrantup.com/downloads.html)
4. Vagrant-bindfs >= 0.3.1 - [Docs](https://github.com/gael-ian/vagrant-bindfs) (Windows users may skip this)

## Installation

1. Download/fork/clone this repo to your local machine.
2. Edit `/bedrock-ansible/Vagrantfile` and set the `VM_HOSTNAME` parameter
3. Edit `/bedrock-ansible/group_vars/development` and update the values from `example.com` to what you specified in `VM_HOSTNAME`
4. Run `vagrant up` within `/bedrock-ansible`
5. Navigate to `http://{VM_HOSTNAME}/wp/wp-login.php` and log in with username `admin` password `admin`
6. Activate the `roots` theme
7. Install `grunt-cli` globally with `sudo npm install -g grunt-cli`
8. Navigate to the theme directory, then run `npm install`

# Sources

Main roots website [http://roots.io/](http://roots.io/)

Bedrock git [https://github.com/roots/bedrock](https://github.com/roots/bedrock)

Roots theme docs [http://roots.io/docs/](http://roots.io/docs/)

Roots theme git [https://github.com/roots/roots](https://github.com/roots/roots)