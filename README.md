Role Name
=========

Role for creating the database and users (database and os) of this application

Requirements
------------

Role Variables
--------------

node_version: Node.js version to install

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

oscbco.dev
