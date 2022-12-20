# Setting up Sonarqube through Ansible

This repository contains a full ansible setup which is capable of setting up and configuring Sonarqube a single server (Additional database hosts possible)

## Prerequisites

Roles which are not dedicated for this job are loaded as submodules and should be initialized with
> git submodule init

## Getting Started

For a detailed documentation of the Sonarqube role, see [roles/sonarqube/README.md](roles/sonarqube/README.md).  
For a detailed documentation of the PostgreSql, see [roles/postgresql/README.md](roles/postgresql/README.md)

You should provide your own inventory and replace the [inventory](./inventory) file. Also change the credentials according to your needs.
Also refer to the [ansible.cfg](./ansible.cfg) file for credential and user configuration.
You also should copy the [defaults/main.yml](/roles/sonarqube/defaults/main.yml) file from the [sonarqube](roles/sonarqube) role and adjust it.  
For getting an overview have a look at the [host_vars/sonar.dev.klackwerk.de.yml](host_vars/sonar.dev.klackwerk.de.yml) file.
