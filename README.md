apt-proxy
=========

This role just adds proxy configuration for APT


Role Variables
--------------

 - config_dir: default /etc/apt/apt.conf.d/
 - config_file: default 99proxy
 - proxy_url: mandatory, but not set, it's up to you

Example Playbook
----------------

    - role: apt-proxy
      proxy_url: http://proxy.server.local:8888


License
-------

GPLv3+

Author Information
------------------

This role was written by Dmitrii Kashin aka freehck
