# vagrant-apache-php-typo3-ansible

Author: AREA-NET GmbH, Markus Schmid www.area-net.de | www.app-agentur-bw.de

* Ubuntu (latest stable)
* ImageMagick, Node/NPM
* Apache 2.4
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


## MIT License

The MIT License (MIT)

Copyright (c) 06.11.2015 AREA-NET GmbH, App-Agentur BW, Markus Schmid

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
