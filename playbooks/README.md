Devil Bird
=====================
This repository contains all of the Ansible-based
playbooks used for Twisted Living staging activities


    devilbird/
    |-- ansible.cfg         # The main ansible configuration file.
    |-- bin/                # Generic utility scripts used by Ansible
    |-- docs/               # Generic docs place
    |-- inventory/          # All inventory file and scripts must be here.
    |   -- group_vars/      # Variables to apply to 'groups' go here.
    |   -- host_vars/       # Variables to apply to individual hosts go here.
    |-- library/            # Custom or non-core modules go here.
    |-- playbooks/          # All of our playbooks go in sub-directories here.
    |-- roles/              # All actual role code goes here.


