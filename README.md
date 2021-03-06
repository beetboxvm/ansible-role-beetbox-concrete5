# Ansible Role: Beetbox Concrete5

[![CircleCI](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-concrete5.svg?style=svg)](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-concrete5)

An Ansible role that creates and installs a Concrete5 project on beetbox.

## Requirements

This role is specifically developed as an extension to beetbox -- https://github.com/drupalmel/beetbox

## Role Variables

Available variables are listed below, along with default values:

Create new Concrete5 project.

    c5_checkout: no
    
Concrete5 project git respository.
    
    c5_repo: "https://github.com/concrete5/concrete5.git"

Concrete5 project version. This can be the full 40-character SHA-1 hash, the literal string HEAD, a branch name, or a tag name.

    c5_version: "HEAD"

Concrete5 checkout depth. git is history truncated to the specified number or revisions.

    c5_checkout_depth: 1

Install Concrete5.

    c5_install: no
    
Concrete5 starting point.
    
    c5_starting_point: "elemental_full"
    
Concrete5 admin account email.
    
    c5_admin_mail: "admin@example.com"
    
Concrete5 admin account password.
    
    c5_admin_password: password
    
Concrete5 locale.
    
    c5_default_locale: "en_US"


# beetbox

https://github.com/beetboxvm/beetbox

## Requirements

* [Vagrant](https://www.vagrantup.com/) >= 1.8
* [Virtualbox](https://www.virtualbox.org/)
* [Vagrant Hostsupdater](https://github.com/cogitatio/vagrant-hostsupdater)
* [Vagrant Auto-network](https://github.com/oscar-stack/vagrant-auto_network)

## Quickstart

  1. Open terminal (or [git bash](https://msysgit.github.io/) for windows users) and run the following commands --

  ```
  git clone https://github.com/beetboxvm/ansible-role-beetbox-concrete5.git concrete5 && cd $_
  vagrant up
  ```

  2. Go to http://concrete5.local/

  ```
  username: admin
  password: admin
  ```

## License

MIT
