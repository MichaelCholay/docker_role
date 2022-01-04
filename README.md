Role Name
=========

docker_role : Installation of docker on ubuntu or centos distribution.

Requirements
------------

No specific requirements.

Role Variables
--------------

No specific variables environments.

Dependencies
------------

No specific dependencies.

Example Playbook
----------------

```yml
- hosts: prod
  become: true
  roles:
    - docker_role

  tasks:
    - name: "Launch nginx container for docker verification"
      docker_container:
        name: webapp
        image: nginx
        ports:
          - "80:80"
```

License
-------

BSD

