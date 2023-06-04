# KodeKloud e-commerce deployment using Ansible

This repository deploys the sample [e-commerce app](https://github.com/kodekloudhub/learning-app-ecommerce) created by KodeKloud using ansible.

## How does it work?

Run an ansible playbook to configure the server.

## How can I use?

1. Change the configurations in the **inventory** file. Replacing the **ip** and **user**.
2. Change the password variable in **group_vars/all** file.
3. Run the playbook:
```
ansible-playbook -i inventory commerce.yml
```

## What will be installed?
- MariaDB as Database.
- Apache2 as WebServer.
- KodeKloud e-commerce sample app written in PHP.

Note: The web and database roles are installed on the same server. This is not recommended in production environments.