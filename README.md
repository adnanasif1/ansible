# Ansible Overview

## What is Ansible?

Ansible is an open-source automation tool that simplifies IT tasks such as configuration management, application deployment, and task automation using simple YAML files known as playbooks.

## Key Features

- **Agentless Architecture**: Ansible operates over SSH and does not require any agent installation on target machines, simplifying management.
- **Declarative Language**: Define the desired state of your systems using YAML, making it easy to read and write.
- **Idempotence**: Ansible ensures that operations are only applied when necessary, preventing unintended changes and ensuring consistency.
- **Extensible**: With a rich ecosystem of modules, you can extend Ansible's capabilities to suit your needs.

## Basic Components

- **Playbook**: A YAML file containing a series of tasks to be executed on target hosts.
- **Inventory**: A file listing the hosts and groups of hosts that Ansible manages.
- **Modules**: Reusable units of work that Ansible executes (e.g., installing packages, managing services).
- **Roles**: A way to organize playbooks and reusable code into structured directories.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# my ansible
  -- install ansible
  -- setup ssh b/w ansible server (host) and target machines (A password less access)
## Inventory
  - Create inventory file put target ips
## playbooks VS adhoc commands
  - For simple command you can use ansible adhoc commands e.g **ansible -i inventory all -m "shell" -a "touch mytextfile.txt"**
  - **BUT**
  - For complex task we usually write playbooks to perform the tasks **ansible-playbook -i inventory myfirst-playbook.yml**
