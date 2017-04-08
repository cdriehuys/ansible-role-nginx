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

nginx_user: nginx
nginx_user_groups: []

nginx_conf_path: /etc/nginx/nginx.conf      # Path to main nginx config file
nginx_site_conf: /etc/nginx/sites-availabe/{{ inventory_hostname }}.conf
nginx_enabled_sites_dir: /etc/nginx/sites-enabled

nginx_site_root: /var/www/{{ inventory_hostname }}
nginx_site_root_mode: 0755
nginx_site_root_file_mode: 0644

nginx_site_servers: []

# Here's an example server entry
nginx_site_servers:
  - name: example.com
    listen: 80
    extra_params: |
        location / {
            alias /path/to/files;
        }
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
