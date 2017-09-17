ansible_role_asciinema
======================

This is a simple Ansible role that installs/uninstall the asciinema utility.
Asciinema is a tool used to record and share your terminal sessions, the right way.
Variables
---------

```yaml
asciinema_installed: true
```

 * asciinema_installed: Default: true. Put false to uninstall the asciinema.

Example Playbook
----------------

See below an example of usage for the module.

```yaml
    - hosts: localhost
      connection: local
      become: true
      roles:
         - { role: mauromedda.ansible_role_epel }
         - { role: mauromedda.ansible_role_asciinema, asciinema_installed: true }
```

License
-------

BSD

Author Information
------------------

Mauro Medda < medda.mauro at gmail dot com >
