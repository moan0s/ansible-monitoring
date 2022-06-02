# Configuring the Ansible playbook

To configure the playbook, you need to have done the following things:

- have a server where monitoring services will run
- [configured your DNS records](configuring-dns.md)
- [retrieved the playbook's source code](getting-the-playbook.md) to your computer

You can then follow these steps inside the playbook directory:

1. create a directory to hold your configuration (`mkdir inventory/host_vars/matrix.<your-domain>`)

1. copy the sample configuration file (`cp examples/vars.yml inventory/host_vars/matrix.<your-domain>/vars.yml`)

1. edit the configuration file (`inventory/host_vars/matrix.<your-domain>/vars.yml`) to your liking. You may also take a look at the various `roles/ROLE_NAME_HERE/defaults/main.yml` files and see if there's something you'd like to copy over and override in your `vars.yml` configuration file.

1. copy the sample inventory hosts file (`cp examples/hosts inventory/hosts`)

1. edit the inventory hosts file (`inventory/hosts`) to your liking


For a basic Matrix installation, that's all you need.