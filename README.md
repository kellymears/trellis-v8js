# Trellis v8js

Work-in-progress.

Ansible role to configure PHP with the php-v8js extension.

This role is made to be used with [Trellis](https://github.com/roots/trellis).

## Get Started

Install the role:

```sh
ansible-galaxy install kellymears.trellis_v8js
```

Add the role to `galaxy.yml`:

```yml
- name: trellis-v8js
  src: kellymears.trellis_v8js
  version: 0.1.0
```

Run `ansible-galaxy install -r requirements.yml` to install the new role.

Then, add the role into both server.yml **and** dev.yml:

```yml
roles:
    - { role: trellis-v8js, tags: [v8, php] }
```

You should add the role right after the Trellis `php` installation.
