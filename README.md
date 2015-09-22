Role for Rails development
==========================

This role will get the target user ready for rails development. Ruby is installed into
the home dirctory using rbenv and ruby-install. 

Role Variables
--------------

  - user: Target user. Ruby and rbenv are installed for this user. 
  - ruby_version: Ruby version to install


Dependencies
------------

  - Antisthenes.ruby

Example Playbook
----------------

This is mainly used to provision vagrant virtual machines for ruby development. It looks like this: 

  - hosts: all
    roles: 
      - role: Antisthenes.rails
        user: vagrant
        ruby_version: 2.2.3

License
-------

MIT
