Role Name
=========

ansible-role-memcache-setup


Requirements
------------
This playbook has a setup task that installs build-essentials if
Debian based distros are found and Devlopment Tools if RedHat Based distros are found

Role Variables
  Memcache Port 2 and 3 can be uncommented .under defaults/main.yml
  to add multiple instances of memcached on the same servers

  memcached_port: '666'
  memcached_port2: '888'
  memcached_port3: '999'
  memcached_listen_ip: 127.0.0.1

Dependencies
------------
 glibc and make tools are required to install memcached from souces. Dependancies are checked and installed during initial play.

Test Playbook

 ansible-playbook -i inventory/docker
 roles/memcache/main.yml

License
---
BSD

Author Information
 Twitter: @TechGameTeddy
