ECGALAXY readyapi role
========

Ansible role which installs ReadyAPI

Requirements
------------

None.


Role Variables
--------------

- `readyapi_version`: the version to download
- `readyapi_url`: the URL from where to download the SH install script
- `readyapi_role_working_dir`: the location on where to store temporary files
- `readyapi_install_dir`: the location on where to install ReadyAPI
- `readyapi_cleanup`: set to `true` (default) to clean up temporary files
- `readyapi_uninstall`: set to `true` to uninstall


Dependencies
------------

- ecgalaxy.common_packages
- ecgalaxy.java_openjdk


Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.readyapi

One-liner
---------

    bash <(curl -s https://code.europa.eu/-/snippets/1/raw/main/ansible-role.sh) ecgalaxy.readyapi

See [ansible-role](https://code.europa.eu/-/snippets/1) for instructions.

Please verify the script integrity first.

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

[ECGALAXY](https://code.europa.eu/groups/ecgalaxy/-/wikis/home) team.
