# Catapult project examples

This repository contains examples of Catapult projects. Each project is a separate directory that contains a `README.md` file with a description of the project and instructions on how to build and run it. It can be a good starting point when building your own project from scratch. Since Catapult is using Ansible a project usually contains the following items:

- `inventory files` that point to a local file and/or to [Providentia](https://github.com/ClarifiedSecurity/Providentia) as inventory source
- `group_vars` directory with variables that are used by the playbooks
- `host_vars` directory with variables that are used by the playbooks
- `roles` directory with universal roles that are specific to the project
- `vm` directory with target specific roles (eg. web_server, file_server, domain_controller etc.)

Check out the project folders in this repository for examples of how to structure your own project.
