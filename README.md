Role Name
=========

Role for creating the database and users (database and os) of this application

Requirements
------------

Role Variables
--------------

userdba: The owner of the database
userweb: The service account for the application
db: The name of the database

Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
            role: oscbco.create_database_and_users,
            userdba: "app-dba",
            userweb: "app-web",
            db:      "app-db"
          }

License
-------

MIT

Author Information
------------------

oscbco.me
