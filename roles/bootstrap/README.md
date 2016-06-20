Role: bootstrap
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

  - `bootstrap_foo` - Required by `bootstrap` role.
  - `bootstrap_dependency_bar_baz` - Required by dependency `bootstrap-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # bootstrap: entry point for defaults
    bootstrap_foo: true

  - `bootstrap_foo` - Allows foo-barring for bootstrap.

Dependencies
------------

This role depends on the following roles:

  - `bootstrap-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the bootstrap role

    - hosts: foo

      roles:
        - bootstrap

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 YOUR NAME HERE

[1]: http://choosealicense.com/licenses/mit/
