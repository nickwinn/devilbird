Role: nyan\_cat
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

  - `nyan_cat_foo` - Required by `nyan_cat` role.
  - `nyan_cat_dependency_bar_baz` - Required by dependency `nyan_cat-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # nyan_cat: entry point for defaults
    nyan_cat_foo: true

  - `nyan_cat_foo` - Allows foo-barring for nyan_cat.

Dependencies
------------

This role depends on the following roles:

  - `nyan_cat-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the nyan_cat role

    - hosts: foo

      roles:
        - nyan_cat

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 Nicholas Winn

[1]: http://choosealicense.com/licenses/mit/
