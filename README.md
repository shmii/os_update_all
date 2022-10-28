# Ansible Role: os-update all
Ansible role to update an OS)


This role update all packages on the OS.


## Test and run environement


```
molecule 4.0.3 using python 3.10 
    ansible:2.10.8
    delegated:4.0.3 from molecule
    docker:2.1.0 from molecule_docker requiring collections: community.docker>=3.0.2 ansible.posix>=1.4.0

```


## Requirements

None.

## Role Variables

vailable variables are listed below, along with default values (see `defaults/main.yml`):

### No vars needed for this role

## Dependencies

None.

## Example Playbook

```yaml
    - hosts: server
      roles:
        - { role: shmii.os-update-all }
```

## Warning / known bugs

/!\ To validate this role with "molecule" from Ubuntu @ WSL/WSL2 it is necessary to create the folder  `/sys/fs/cgroup/systemd` on the host linux subsystem. 


`sudo mkdir /sys/fs/cgroup/systemd`

This directory is necessary for some os (RHEL9, Rocky9, etc...) and not existing on local Ubuntu WSL sub Systeme. 

## Sources and Bibliography

n/a


## License

GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007

## Author Information

This role was created in 2022 by [Thomas CHALMEL] (https://www.thomas.chalmel.org/).
