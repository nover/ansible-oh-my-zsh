Role Name
=========

oh my zsh installer for Ubuntu and macOS systems. The original work has been taken from here https://github.com/RaymiiOrg/ansible/blob/master/oh-my-zsh/ohmyzsh.yml

I have taken the liberty of converting it into a "real ansible role" and subseqently published it on ansible galaxy.

Requirements
------------

Nothing special except ansible and an Ubuntu or macOS target

Role Variables
--------------

You can control the theme that is being installed, default theme is `steeef`
```yaml
ohmyzsh_theme: 'steeef'
```

Example Playbook
----------------

An example playbook is as follows
```yaml
- hosts: servers
  roles:
      - { role: nover.ohmyzsh, ohmyzsh_theme: 'robbyrussell' }
```

License
-------

GitHub The Unlicense
