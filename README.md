docker-swarm-node
=========

Install and configure a docker swarm node for Ubuntu trusty and add to an existing swarm cluster using consul.

Requirements
------------

none

Role Variables
--------------

- `docker_user` : linux username for docker.
- `consul_ip` : IP address of the consul server
- `docker_apt_key` : key id for apt-key. (see https://get.docker.com and search "--recv-key" in page.)

Dependencies
------------

none

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: hidekuro.docker, docker_user: "youruser" , consul_ip: "conulserverip"}

License
-------

MIT

Tested on
---------

Ubuntu 14.04 trusty tahr
