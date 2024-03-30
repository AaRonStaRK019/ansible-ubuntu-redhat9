## Hosting Web Servers on different Ansible nodes - Ubuntu and RedHat Linux  - using AMazon EC2


`Spin Up 3 EC2 Instances - Ubuntu(control), Ubuntu(slave node-1) and RedHat(slave node-2)`

![EC2 Instances](./img/start-3-instances.png)


`install ansible on control node`

![](./img/install-ansible-on-control.png)


`confirm ansible installation on control node`

![](./img/confirm-ansible-installation.png)

`clone website repository to master node`

![](./img/clone-website-fles-to-master.png)

`add IP addresses of slave nodes to inventory file`

![inventory file](./img/inventory-file.png)


`run a ping test to confirm connection to ansible nodes`

![ping test](./img/ping-test-success.png)


`confirm that apache2 isn't yet installed on the apache-server node`

![no apache2](./img/confirm-no-apache2-ubuntu.png)


`confirm that Apache httpd isn't yet installed on redhat-server node`

![no httpd](./img/confirm-no-httpd-redhat.png)


`write and run a playbook to install apache2 on the ubuntu server node, and apache httpd on the redhat server node`

[installation playbook](./playbooks/install_web_servers.yml)

![run installation playbook](./img/run-installation-playbook.png)


`Confirm that apache2 and httpd are installed and working`

![apache2 active](./img/confirm-apache2-working-ubuntu.png)

![apache2 active](./img/default-page-ubuntu.png)


![httpd active](./img/confirm-httpd-working-redhat.png)

![httpd active](./img/default-page-redhat.png)


`write and run a playbook to copy the website files to the ansible nodes`

[copy playbook](./playbooks/copy_web_files.yml)

![run copy playbook](./img/copy-files-to-nodes.png)


`confirm web files are in /var/www/html directory on both nodes`

`ubuntu server - files`

![ubuntu-seerver web files](./img/confirm-copy-ubuntu.png)

`redhat server - files`

![redhat-server web files](./img/confirm-copy-redhat.png)


`reload servers IP addresses and check for newly-hosted page`

`ubuntu-hosted page`

![ubuntu hosted page](./img/ubuntu-server-working.png)

`redhat-hosted page`

![redhat hosted page](./img/redhat-server-working.png)
