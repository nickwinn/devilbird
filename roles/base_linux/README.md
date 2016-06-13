Role: base\_linux
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

  - `base_linux_foo` - Required by `base_linux` role.
  - `base_linux_dependency_bar_baz` - Required by dependency `base_linux-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # base_linux: entry point for defaults
    base_linux_foo: true

  - `base_linux_foo` - Allows foo-barring for base_linux.

Dependencies
------------

This role depends on the following roles:

  - `base_linux-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the base_linux role

    - hosts: foo

      roles:
        - base_linux

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 YOUR NAME HERE

[1]: http://choosealicense.com/licenses/mit/
