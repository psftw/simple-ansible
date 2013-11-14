simple-ansible
=================

Some simple Ansible playbooks you may find useful.

* build.yml: CentOS6-based continuous integration toolkit

    * GitLab 6.2, heavily based on the [gitlab-recipe][1] for CentOS
    * Jenkins
    * Python 2.7 ecosystem thanks to the [PUIAS][2] Computational repository.
    * Haskell ecosystem thanks to the [justhub.org][3] repository.
    * Node.js

* License: MIT

[1]: https://github.com/gitlabhq/gitlab-recipes/tree/master/install/centos
[2]: http://springdale.math.ias.edu/wiki/YumRepositories6
[3]: http://www.justhub.org

Status
---------

Works well enough for me, but still needs polish such as driving more configuration through
variables.

Quick Start
------------

* Bootstrap a CentOS6.4 system
* Review/modify build.yml and hosts
* Execute build.yml with Ansible 1.3+
* Execute some interactive commands which I have not bothered to automate

        # cd /etc/nginx
        # openssl req -new -x509 -nodes -days 3560 -out gitlab.crt -keyout gitlab.key
        # su git
        $ cd /home/git/gitlab
        $ bundle exec rake gitlab:setup RAILS_ENV=production
        $ exit
        # service gitlab start

* Default GitLab credentials: admin@local.host/5iveL!fe
