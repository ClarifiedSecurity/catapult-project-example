# Catapult project example

This repository is an example of a Catapult project. It can be a good starting point when building your own project from scratch. Since Catapult is using Ansible a project usually contains the following items at a minimum:

- `inventory files` that point to a local file and/or to [Providentia](https://github.com/ClarifiedSecurity/Providentia) as inventory source
- `group_vars` directory with variables that are used by the playbooks
- `host_vars` directory with variables that are used by the playbooks
- `roles` directory with universal roles that are specific to the project
- `vm` directory with target specific roles (eg. web_server, file_server, domain_controller etc.)

The project has an example host called `monolith` that can be used to set up Vault/Keycloak/Providentia/Nexus on a pre-existing VM. Just fill out the required variables in `host_vars/monolith.yml` and run `ctp host deploy monolith`.

Refer to [Catapult Docs](https://clarifiedsecurity.github.io/catapult-docs/catapult/01-installation/) for full documentation.
