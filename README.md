Nagios 4
========

Builds and installs nagios core from source.

Role Variables
--------------

- `nagios_web_password` - The 'user one' password for Nagios' web interface. Defined as a default, should be overrided in `vars/main.yml`.
- `nagios_version` - Expected from the global scope, defines the nagios core version to build and install.
- `nagios_plugins_version` - Expected from the global scope, defines the nagios plugins version to build and install.

Dependencies
------------

The [common role](https://git.forgeservicelab.fi/ansible-roles/common) is defined as a dependency, make sure it is present in your playbook.

Author Information
------------------

[Forge Servicelab Team](http://forgeservicelab.fi)
