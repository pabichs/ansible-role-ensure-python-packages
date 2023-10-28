ensure_python_packages
=========

This role serves `ansible.builtin.pip` module as a role.

Requirements
------------

None.

Role Variables
--------------

| Variable                    | Required | Default     | Description                                                                       |
|-----------------------------|----------|-------------|-----------------------------------------------------------------------------------|
| `python_packages`           | no       | _undefined_ | List of python packages to install. Passes all arguments to `ansible.builtin.pip` |                                                              


Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: pabichs.ensure_python_packages
      become: false
      vars:
        python_packages:
          - name: yt-dlp
            version: 2023.10.13
```

License
-------

BSD, MIT

Author Information
------------------

Created in 2023
