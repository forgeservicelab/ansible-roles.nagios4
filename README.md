Nagios 4
========

Builds and installs nagios core from source.
Needs ansible version >= 1.6

Role Variables
--------------

- `nagios_web_password` - The 'user one' password for Nagios' web interface. Defined as a default, should be overrided in `vars/main.yml`.
- `nagios_version` - Expected from the global scope, defines the nagios core version to build and install.
- `nagios_plugins_version` - Expected from the global scope, defines the nagios plugins version to build and install.
- `nrpe_version` - Expected from the global scope, defines the nrpe version to build and install.
- `is_core` - Expected from the global scope, defines whether the target host will serve nagios core or it will be a monitored node.
- `build_tools` - List of development packages needed to build nagios and companions from source (Distribution dependent).
- `ssl_libs` - Name of the development package for OpenSSL (Distribution dependent).
- `ldap_libs` - Name of the development package for LDAP (Distribution dependent).
- `mysql_libs` - Name of the devemlopment package for MySQL (Distribution dependent).
- `apache` - Name of the apache webserver package (Distribution dependent).
- `gd` - Name of the GD library package (Distribution dependent).
- `gd_dev` - Name of the development package for GD (Distribution dependent).
- `php` - List of php packages needed to run nagios (Distribution dependent).

Dependencies
------------

The [common role](https://git.forgeservicelab.fi/ansible-roles/common) is defined as a dependency, make sure it is present in your playbook.

Author Information
------------------

[Forge Servicelab Team](http://forgeservicelab.fi)
