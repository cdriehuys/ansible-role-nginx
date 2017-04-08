cdriehuys.nginx
=========

Install and configure NGINX.

Requirements
------------

None.

Role Variables
--------------

The following are the variables used by the role and their defaults.

```YAML
apt_cache_time: 3600
```

```YAML
nginx_user: nginx
nginx_user_groups: []
```

Allows for changing the user that runs the nginx process as well as the groups
that the user belongs to.

Dependencies
------------

None.

Example Playbook
----------------

To run the role, include it as follows.

    - hosts: all
      roles:
         - cdriehuys.nginx

License
-------

MIT

Author Information
------------------

Chathan Driehuys (cdriehuys@gmail.com)
