# Ansible Role: homer-docker

Ansible role to create homer docker container.

## Mandatory Role Variables

This role requires you to set the address on which homer should listen.

```
homer_docker__listen_address: "{{ ansible_host }}"
```

The container will be exposed to the _homer_docker__listen_address_ on port 33099.

It is recommended to update Homer regurarly. Set the docker image version:

```
homer_docker__homer_version: "21.09.2"
```

The assets which are rendered by Homer are read from a git repository:

```
homer_docker__assets_git_repo_url: "https://github.com/user/some-assets-repo"
```

## Optional Role Variables

Possible optional role variables can be found in [defaults/main.yml](defaults/main.yml).