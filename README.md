linux_base
========

Install Imagemacgick and its dependencies.  Also, updates apt cache

This role is used to install the imagemagick package and its dependencies on a server running Ubuntu 12.04LTS.

```
- name: Imagemagick | Update apt
  apt: update_cache=yes
  sudo: yes

- name: Imagemagick | Install Imagemagick
  action: apt pkg={{ item }} state=latest
  sudo: yes
  with_items:
    - imagemagick
    - libmagickcore-dev
    - libmagickwand-dev
```

Requirements
-----------
Operating system developed for: Linux (Ubuntu 12.04LTS 64 bit)

Role Variables
-----------
No Variables for this playbook

Dependencies
-----------
None

License
-----------
GPL v3