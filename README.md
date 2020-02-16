# Trellis v8js

Work-in-progress.

Ansible role to configure PHP with the php-v8js extension.

This role is made to be used with [Trellis](https://github.com/roots/trellis).

## Get Started

Add the role to the requirements.yml file of Trellis :

```yml
- name: trellis-v8js
  src: kellymears.trellis-v8js
  version: 0.1.0
```

Run `ansible-galaxy install -r requirements.yml` to install the new role.

Then, add the role into both server.yml **and** dev.yml:

```yaml
roles:
    ... other Trellis roles ...
    - { role: trellis-v8js, tags: [v8, php]}
```
