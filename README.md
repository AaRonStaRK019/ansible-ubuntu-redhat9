## Hosting Web Servers on different Ansible nodes - Ubuntu and RedHat Linux

`The aim of this exercise will be to host a mockup fitness sign-up page on two ansible nodes (Ubuntu and RedHat Linux), using apache2 and apache httpd respectively`

`Ansible playbooks used:`

`Install web servers on both nodes`

[Install webservers PLaybook](./playbooks/install_web_servers.yml)

`Copy  web files to /var/www/html directory on both nodes`

[Copy webpage files PLaybook](./playbooks/ansible_copy_files.yml)
