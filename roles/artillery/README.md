Role: artillery
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

  - `artillery_foo` - Required by `artillery` role.
  - `artillery_dependency_bar_baz` - Required by dependency `artillery-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # artillery: entry point for defaults
    artillery_foo: true

  - `artillery_foo` - Allows foo-barring for artillery.

Dependencies
------------

This role depends on the following roles:

  - `artillery-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the artillery role

    - hosts: foo

      roles:
        - artillery

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 YOUR NAME HERE

[1]: http://choosealicense.com/licenses/mit/
