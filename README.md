Duologic.statsdaemon
====================

This role configures and installs statsdaemon with the OS package manager.

Requriments
-----------

You probably need to add a repository that has the statsdaemon package for your distribution. I've used raintaink's PackageCloud. See the example Playbook.

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: packagecloud, repository: raintank/raintank, os: centos, version: 7 }
         - { role: Duologic.statsdaemon }
```

License
-------

MIT

Author Information
------------------

Jeroen Op 't Eynde, jeroen@simplistic.be
