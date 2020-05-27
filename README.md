# vagrant-kops

(c) Andre Lohmann (and others) 2020

## Maintainer Contact
 * Andre Lohmann
   <lohmann.andre (at) gmail (dot) com>

## content

This vagrant machine will use kops to deploy a k8s cluster on aws

## Prequesites

### VirtualBox

  * install the latest virtualbox from oracle repositories (https://www.virtualbox.org/wiki/Downloads)
  * if you are on a linux distro, follow the instructions to add the oracle repo
  * install the latest Oracle VM VirtualBox Extension Pack

### Vagrant

#### cli

  * Install the latest vagrant (https://www.vagrantup.com/downloads.html)

#### plugins

the vagrant machines depends on the following vagrant plugin.

```
vagrant plugin install vagrant-vbguest
```

this pluin should get installed automatically on a "vagrant up", if that fails anyways, please manually install the plugin by entering the command

### AWS

  * Create IAM User (with FullAdmin permissions preferred)
  * fetch Programmatic Access Credentials

## usage

### upstart

  * clone the repo and change to the directory
  * copy ansible_vagrant/custom_vars.yml.example to ansible_vagrant/custom_vars.yml and set your credentials
  * run the machine

```
vagrant up
```
