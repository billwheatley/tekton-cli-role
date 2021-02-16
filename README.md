tekton-cli-role
===============
Ansible role to install the x86 Tekton CLI (via tarball). This will also install bash completion for `tkn` (Tekton CLI) as well.

This was also designed as part of a desktop provisioning playbooks found here <https://github.com/billwheatley/provision-desktop>

After using this role you should have `tkn` in your path and ready to use.  For bash completion any new bash shells launched after using this role will have completion capabilities (assuming you meet the requirements).

Requirements
------------

- If you want bash completion you must have distribution with `dnf` or `yum` or `apt` package manger OR the bash completion package installed if you are using a different package manager.

Role Variables
--------------

none

Example Playbook
----------------

```yaml
- name: My Playbook
  hosts: desktop
  roles:
    - role: tekton-cli-role
```

License
-------

GPLv2

Author Information
------------------

Contact via [Github](https://github.com/billwheatley/)
