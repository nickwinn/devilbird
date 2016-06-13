Role: apache2
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

  - `apache2_foo` - Required by `apache2` role.
  - `apache2_dependency_bar_baz` - Required by dependency `apache2-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # apache2: entry point for defaults
    apache2_foo: true

  - `apache2_foo` - Allows foo-barring for apache2.

Dependencies
------------

This role depends on the following roles:

  - `apache2-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the apache2 role

    - hosts: foo

      roles:
        - apache2

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 YOUR NAME HERE

[1]: http://choosealicense.com/licenses/mit/
