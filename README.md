ImageMagick
========

This Ansible role is used to install the ImageMagick apt package and its dependencies on a server running Ubuntu 12.04LTS.

## Installation

``` bash
$ ansible-galaxy install crushlovely.imagemagick
```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
---
- hosts: localhost
  roles:
    - { role: crushlovely.imagemagick }
```

## Dependencies

None

## License

MIT
