Role: dns
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

  - `dns_foo` - Required by `dns` role.
  - `dns_dependency_bar_baz` - Required by dependency `dns-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # dns: entry point for defaults
    dns_foo: true

  - `dns_foo` - Allows foo-barring for dns.

Dependencies
------------

This role depends on the following roles:

  - `dns-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the dns role

    - hosts: foo

      roles:
        - dns

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 YOUR NAME HERE

[1]: http://choosealicense.com/licenses/mit/
