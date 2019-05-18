Role Name
=========

Role for creating the database and users (database and os) of this application

Requirements
------------

Role Variables
--------------

userdba: The owner of the application database
db: The name of the database
postgresql_version: This version is used to find the pg_hba.conf file
userdba_password: The password for the dba

Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
            role: oscbco.create_database_and_users,
            userdba: "app-dba",
            userdba_password: $ANSIBLE_VAULT;...,
            userweb: "app-web",
            db:      "app-db",
            postgresql_version: 11
          }

License
-------

MIT

Author Information
------------------

oscbco.me
