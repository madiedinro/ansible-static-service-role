# Asible role for static service (frontend)

## Usage

Build for Ubuntu!
Add to ansible playbook following:

    - import_role:
        name: dr.static-service
      vars:
        # service name
        dr_name: my-static
        # [dir mode]
        dr_dir_mode: 0755
        # [path to deploy]
        dr_dir: '/srv/{{dr_name}}'
        # git repo
        dr_repo: https://github.com/myyyyyyy
      tags: ['static']
      become: yes

## Default parameters

Discover in `defaults/main.yml`
