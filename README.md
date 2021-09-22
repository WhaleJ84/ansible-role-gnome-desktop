Gnome Settings
=========

Configures Gnome settings for the user.

Requirements
------------

The following collections are required:

- community.general

They can be installed by running `ansible-galaxy collection install $COLLECTION`.

Role Variables
--------------

The role will optionally install Dconf Editor to help in development:

- install\_editor: False

Other variables are stored in `vars/main.yml`.

Example Playbook
----------------

    - hosts: localhost
      roles:
         - { role: whalej84.gnome-settings, install_editor: True }

