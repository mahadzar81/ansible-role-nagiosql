# Ansible Role: NagiosQL

## Installation
Use ansible-galaxy command to download this repository to the system that will run this playbook.

```
ansible-galaxy install mahadzar81.nagiosql
```

## Requirements
This role will install nagios and nagiosQL (web based configuration tool for Nagios ) onto your nodes.
No special requirements; note that this role requires root access, so either run it in a playbook with a global `become: true`, or invoke the role in your playbook like:

```
- name: "Provision Nagios and NagiosQL server"
  hosts: all
  gather_facts: yes
  become: true
  roles:
    - { role: ansible-role-nagiosql }

```
