Ansible Playbook: postgresql-dbsw-compile
=========================================

Compile PostgreSQL database server software

Supported OS:
-------------
* RedHat
* CentOS
* OracleLinux

Requirements
------------

This playbook requires the postgresql-dbsw-compile role.

`$ ansible-galaxy install -r roles/requirements.yml`

Examples
--------

    $ ansible-playbook playbook.yml --list-tasks
    $ ansible-playbook playbook.yml --list-tags

Complete Postgres software compilation

    $ ansible-playbook playbook.yml

Install required dev packages

    $ ansible-playbook playbook.yml --tags=postgresql_dbsw_compile_required_packages

Create compile_from_source.sh script only

    $ ansible-playbook playbook.yml --tags=postgresql_dbsw_compile_create_compile_script

Fetch compiled binaries back to Ansible control machine

    $ ansible-playbook playbook.yml --tags=postgresql_dbsw_compile_fetch_compiled_binaries



License
-------

GPLv3 - GNU General Public License v3.0

Author Information
------------------

This playbook was created in 2018 by [Krzysztof Lewandowski](mailto:Krzysztof.Lewandowski@fastmail.fm).


