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
      tags: ['my-static']
      become: yes

params:

- **drs_setup_user:** (yes/no) do setup additional user
- [**drs_user:** (str)] create additional user with sudo
- [**drs_pass:** (str)] new user passwords
- [**def_user_key_file:**] (str) path to public key
- [**drs_data_dir:**] (str) directory outside home that can be used by added user

## Default parameters

Discover in `defaults/main.yml`
