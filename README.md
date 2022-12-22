### Ansible Playbook:
*****************
---
- name: abc install & start services
  hosts: all (create the hosts and put your instances ip address)
  become: true

  tasks:
  - name: install abc
    yum:
      name: abc
      state: latest

  - name: start abc
    service:
      name: abc
      state: started
Footer
© 2022 GitHub, Inc.
