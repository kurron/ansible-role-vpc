Role Name
=========

Installation of Java runtimes than any self-respecting JVM developer loves and needs.

Requirements
------------

TODO

Role Variables
--------------

* jvm_oracle_jdk_install: true
* jvm_oracle_jdk_version: jdk1.8.0_111
* jvm_oracle_jdk_path: 8u111-b14/jdk-8u111
* jvm_oracle_jdk_link_destination: oracle-jdk-8
* jvm_azul_jdk_install: false
* jvm_azul_jdk_build: 8.17.0.3
* jvm_azul_jdk_version: 8.0.102
* jvm_azul_jdk_link_destination: azul-jdk-8

Dependencies
------------

* kurron.base

Example Playbook
----------------

```
- hosts: servers
  roles:
      - { role: kurron.jvm-developer, jvm_azul_jdk_install: true, jvm_oracle_jdk_install: false }
```

License
-------

This project is licensed under the [Apache License Version 2.0, January 2004](http://www.apache.org/licenses/).

Author Information
------------------

[Author's website](http://jvmguy.com/).
