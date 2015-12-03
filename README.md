lucazz.symlinks
=========

This is a Ansible role that creates symlinks based on a dict privided previously in a var_file

Role Variables
--------------

By default it'll load the defaults/main.yml file, which contain a dummy set of values for src and dest for this role.
You should set them at play/playbook level instead.
Here's an example of a var_file that could be used:

# defaults file for lucazz.symlinks
symlinks:
    - { src: '/home/vagrant', dest: '/tmp/0' }


Dependencies
------------

There are no dependencies besides Ansible core modules for this role.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - hosts: servers
      sudo: yes
      roles:
         - lucazz.symlinks

License
-------

BSD
