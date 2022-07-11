# File backup automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-filebackup
  name: ansible-role-filebackup
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-filebackup

- Import role and override role variables, e.g.
```
- name: Setup disk
  roles:
    - role: ansible-role-filebackup
```
