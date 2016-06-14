Role: docker
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

  - `docker_foo` - Required by `docker` role.
  - `docker_dependency_bar_baz` - Required by dependency `docker-dependency-bar` role.


Role Variables
--------------

The default role variables in `defaults/main.yml` are:

    ---
    # docker: entry point for defaults
    docker_foo: true

  - `docker_foo` - Allows foo-barring for docker.

Dependencies
------------

This role depends on the following roles:

  - `docker-dependency-bar`


Example Playbook
----------------

    ---
    # This playbook deploys the docker role

    - hosts: foo

      roles:
        - docker

License
-------

[MIT][1]

Author Information
------------------

(c) 2016 - Nick Winn
(c) 2016 YOUR NAME HERE

[1]: http://choosealicense.com/licenses/mit/
