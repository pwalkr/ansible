# Ansible

https://www.ansible.com/

Common tasks and utilities used in my own ansible-managed network

## To Use

Clone to a role directory like `roles/common`, and then include tasks through
said role. E.g.:

    tasks:
      - include_role:
          name: common
          tasks_from: tmp_tmpfs.yml
        # Define any variables required by the module
        vars:
          foo: bar
