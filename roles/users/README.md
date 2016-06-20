Role: users
====
**Description:**

This role will:

- Make your favorite breakfast sandwich

Requirements
------------

**Supports:**

  - CentOS/RHEL

**Assumptions:**

This role makes the assumption that the `foo` command exists on the system.  Ansible installs this with the `foo` role.

**Required Variables:**

  - `users_foo` - Required by `users` role.
  - `users_dependency_bar_baz` - Required by dependency `users-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # users: entry point for defaults
    users_foo: true

  - `users_foo` - Allows foo-barring for users.

Dependencies
------------

This role depends on the following roles:

  - `users-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the users role

    - hosts: foo

      roles:
        - users

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 YOUR NAME HERE

[1]: http://choosealicense.com/licenses/mit/
