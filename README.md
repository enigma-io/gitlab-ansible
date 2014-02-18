gitlab-ansible
==============

Ansible playbooks for installing GitLab 6.5 on Ubuntu 12.04.4 LTS with
PostgreSQL and Nginx.

## Prerequisites

Make sure you've [installed
Ansible](http://ansibleworks.com/docs/gettingstarted.html#getting-ansible). If
you'd like to use the Vagrantfile instead of Ansible directly, make sure
you've [installed Vagrant](https://docs.vagrantup.com/v2/installation/).

Copy `vars/user.yml.example` to `vars/user.yml` and set your domain name
and a PostgreSQL DB password.

## Installation

```bash
$ ansible-playbook -i site.yml
```

or if you'd like to use the Vagrantfile:

```bash
$ vagrant up
```

When the Ansible playbooks have finished running, you should now be able to
login to the GitLab web interface with the default login:

```
Username: admin@local.host
Password: 5iveL!fe
```

## Credits

Originally based on [tingtun /
ansible-playbook-gitlab](https://github.com/tingtun/ansible-playbook-gitlab).

Contributors to this repository include:

* Patrick Stankard (https://github.com/PatrickStankard)

## License

The MIT License (MIT)

Copyright (c) 2014 Enigma Technologies, Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

