# Ansible Role: Beetbox Concrete5

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

## Dependencies

- Beetbox -- https://github.com/drupalmel/beetbox

## License

MIT