# Ansible Role: Docker

[![License](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![GitHub tag](https://img.shields.io/github/tag/OnkelDom/ansible-role-docker.svg)](https://github.com/OnkelDom/ansible-role-docker/tags)
[![GitHub issues](https://img.shields.io/github/issues/OnkelDom/ansible-role-docker)](https://github.com/OnkelDom/ansible-role-docker/issues)
[![GitHub license](https://img.shields.io/github/license/OnkelDom/ansible-role-docker)](https://github.com/OnkelDom/ansible-role-docker/blob/master/LICENSE)

## Description

Install and docker using ansible.

## Requirements

- Ansible >= 2.6 (It might work on previous versions, but we cannot guarantee it)

## Role Variables

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `docker_users` | [] | Define users to manage docker |
| `docker_config` | [defaults](defaults/main.yml) | Define docker config |

### Playbook

```yaml
- hosts: docker
  vars:
    docker_users:
      - onkeldom
  roles:
    - ansible-role-docker
```

## Contributing

See [contributor guideline](CONTRIBUTING.md).

## License

This project is licensed under MIT License. See [LICENSE](/LICENSE) for more details.
