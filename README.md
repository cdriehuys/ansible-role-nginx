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
