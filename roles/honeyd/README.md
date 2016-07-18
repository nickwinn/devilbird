Role: honeyd
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

  - `honeyd_foo` - Required by `honeyd` role.
  - `honeyd_dependency_bar_baz` - Required by dependency `honeyd-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # honeyd: entry point for defaults
    honeyd_foo: true

  - `honeyd_foo` - Allows foo-barring for honeyd.

Dependencies
------------

This role depends on the following roles:

  - `honeyd-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the honeyd role

    - hosts: foo

      roles:
        - honeyd

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 Nicholas Winn

[1]: http://choosealicense.com/licenses/mit/
