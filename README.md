Role Name
=========

Install essential openvpn client, configure and start service.

Requirements
------------

None

Role Variables
--------------

- openvpn_client_user: user name
- openvpn_client_password: password
- openvpn_client_conf_file: path to config file. file name is used for naming serice (es: openvpn@client)


Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      vars:
        openvpn_client_user: 'user'
        openvpn_client_password: 'passwrod'
        openvpn_client_conf_file: /path/to/conf/client.conf
      roles:
         - openvpn-client

License
-------

BSD

Author Information
------------------

Antonio Barbaro <antonio.barbaro@gmail.com>
