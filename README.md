# Asible role for static service (frontend)

## Usage

Build for Ubuntu!
Add to ansible playbook following:

    - import_role:
        name: dr.static-service
      vars:
        dr_name: my-static
        dr_dir: '/srv/{{dr_name}}'
        dr_repo: https://github.com/myyyyyyy
      tags: ['static']
      become: yes

params:

- **dr_name:** (str) service name
- **dr_dir:** (str) path to deploy
- **dr_repo:** (str) git repo

## Default parameters

Discover in `defaults/main.yml`
