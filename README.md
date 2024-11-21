gnome-desktop
=========

Installs and configures gnome-desktop for the user.

Requirements
------------

The following collections are required:

- community.general

They can be installed by running `ansible-galaxy collection install $COLLECTION`.

To include this role in your `requirements.yml` file, add the following list item:

```yaml
---
roles:
  - name: whalej84.gnome-desktop
    src: https://github.com/WhaleJ84/ansible-role-gnome-desktop.git
    scm: git

  - name: whalej84.psutil
    src: https://github.com/WhaleJ84/ansible-role-psutil.git
    scm: git

collections:
  - community.general
```

Role Variables
--------------

The role will optionally install Dconf Editor to help in development:

- install\_editor: False

Other variables are stored in `vars/main.yml`.

Example Playbook
----------------

This example playbook shows how I would use this role, with custom variables to suit my needs.

```yaml
- hosts: localhost

  roles:
    role: whalej84.gnome-desktop
    tags: [ gnome-desktop ]
```

