Ansible role: Laravel tasks.
=========

Configures cron tasks.

Requirements
------------

None.

Role Variables
--------------

    laravel_cron: {}

Dependencies
------------

- shomatan.php-fpm

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: shomatan.laravel
          laravel_cron:
            my_app:
              user: nginx
              path: /var/www/my_app

License
-------

BSD

Author Information
------------------
