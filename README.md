Linux Updates
=========

Install updates on Linux

Role Variables
--------------

```yaml
# defaults file for linux_updates
# When updating systems, a reboot may be required. Here you can select to:
# "yes": Always reboot when packages have changed.
# "no": Never reboot when packages have changed.
update_reboot: yes
```



Example Playbook
----------------


```yaml
- name: Install Linux updates
  hosts: all
  gather_facts: yes
  tasks:
    - name: Apply Linux updates role
      include_role:
        name: itblaked.linux_updates
```


License
-------

BSD

Author Information
------------------

Blake Douglas, blake@redhat.com
