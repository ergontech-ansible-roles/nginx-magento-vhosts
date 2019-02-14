Nginx Magento Vhosts Role
=========

This role sets up a nginx server for magento

Role Variables
--------------

```
# example vars
nginx_snippet_includes:
  - realip.conf
  - x-whom.conf
fqdn:
  - domain: dev.test.com
    code: dev
    type: website
    includes:
      - special-header-file-for-this-site
env: dev
magento_version: "2"
release_pub_dir: /var/www/html
nginx_listen_port: 80
php_fpm_listen: 30
mage_run_mode: yes
```

----------------

```
#   requirements.yml
#
#   Example
# - src: https://github.com/ergontech-ansible-roles/nginx-magento-vhosts
#   version: master
#   name: nginx-magento-vhosts
```

License
-------

[MIT](LICENSE)