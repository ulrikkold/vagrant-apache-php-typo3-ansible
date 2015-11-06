# vagrant-apache-php-typo3-ansible

* Current Ubuntu system
* Apache 2.4 (imagemagick, npm)
* PHP 5.6 (imagick, curl, gd, intl, cli, mysql)
* MySQL (latest stable)
* Xdebug
* Composer
* Typo3 6.2.15

## System requirements

* VirtualBox www.virtualbox.org
* Vagrant www.vagrantup.com
* Ansible www.ansible.com (see next chapter)

## Install Ansible

### Mac OSX

* Install Homebrew http://brew.sh
* Install Ansible with
```
> brew install ansible
```

### Windows

* Tutorial: http://www.azavea.com/blogs/labs/2014/10/running-vagrant-with-ansible-provisioning-on-windows/
* Windows shell provisioning script: https://github.com/geerlingguy/JJG-Ansible-Windows

## Start up

* Download code or repository
* Open console and change into the downloaded folder

```
> vagrant up
```

* Open browser and see the Typo3 installation wizard on http://192.168.33.99
* Optional: Setting hostname.dev in /etc/hosts to 192.168.33.99

## Customizing

Change default vars in ansible/vars/all.yml
* Server hostname
* Server packages
* PHP packages
* Typo3 version
* ...

Re-provision the box after changing vars with

```
> vagrant provision
```
