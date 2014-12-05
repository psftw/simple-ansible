simple-ansible
=================

Some simple Ansible playbooks for CentOS6.

This was an exploration of Ansible + CentOS6 for some build systems, but should
be dismissed since it is unmaintained.  The code is left here for historical
reference.

* build.yml: various tools

    * Jenkins

    * Python 2.7 ecosystem thanks to the [PUIAS][1] Computational repository.

    * Haskell ecosystem thanks to the [justhub.org][2] repository.

    * Node.js

* License: MIT

[1]: http://springdale.math.ias.edu/wiki/YumRepositories6
[2]: http://www.justhub.org

Quick Start
------------

1. Bootstrap a CentOS6 system

1. Review/modify build.yml and hosts

1. Execute build.yml with Ansible 1.3+

