apt-proxy
=========

This role just adds proxy configuration for APT


Role Variables
--------------

 - config_dir: default /etc/apt/apt.conf.d/
 - config_file: default 99proxy
 - http_proxy: mandatory, but not set, it's up to you
 - https_proxy: mandatory, but not set, it's up to you
 - ftp_proxy: not set, it's up to you
 - socks_host: not set, it's up to you
 - no_proxy: mandatory, but not set, it's up to you

Example Playbook
----------------

    - role: apt-proxy
      http_proxy: http://proxy.server.local:8888
      https_proxy: http://proxy.server.local:8888
      no_proxy: http://proxy.server.local:8888


    - role: apt-proxy
      http_proxy: http://proxy.server.local:8888
      https_proxy: http://proxy.server.local:8888
      ftp_proxy: http://proxy.server.local:8888
      socks_host: http://proxy.server.local:8888
      no_proxy: http://proxy.server.local:8888

License
-------

MIT

Author Information
------------------

This role was written by Dmitrii Kashin aka freehck
