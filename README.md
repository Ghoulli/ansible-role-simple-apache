Ansible Role: Simple Apache

A very simple Ansible role to install and start the Apache web server.

Role Variables

These are the default variables, which can be overridden:

apache_package_name: The name of the Apache package. (Default: apache2)

apache_service_name: The name of the Apache service. (Default: apache2)

For Red Hat-based systems, you can override these in your playbook:

- hosts: all
  become: yes
  vars:
    apache_package_name: httpd
    apache_service_name: httpd
  roles:
    - YourUsername.simple_apache_role


Example Playbook

See the playbook.yml in the root of this repository for usage.

License

MIT