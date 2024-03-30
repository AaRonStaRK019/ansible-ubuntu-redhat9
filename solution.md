## Hosting Web Servers on different Ansible nodes - UBuntu and RedHat Linux


`Spin Up 3 EC2 Instances - Ubuntu(control), Ubuntu(slave node-1) and RedHat(slave node-2)`
![EC2 Instances](./img/start-3-instances.png)


`install ansible on control node`
![](./img/install-ansible-on-control.png)


`confime ansible installation on control node`
![](./img/confirm-ansible-installation.png)


2. `change directory using the relative pathname`
![relative pathname](./img-screenshots/b.cd-into-tests-relative.png)


3. `create new file with text in specified directory using echo command`
![echo command](./img-screenshots/c.echo-hello-a-misc-fileA.png)


4. `create empty file in the misc directory, then add dummy content.`
![echo command](./img-screenshots/d.dummy-content--empty-fileB.png)


5. `Copy contents of fileA into fileC`
![cp](./img-screenshots/e.copy-fileA--fileC.png)


6. `Move contents of fileB into fileD`
![mv](./img-screenshots/f.move-fileB--fileD.png)


7. `Create a tar archive called misc.tar for the contents of misc directory`
![tar -cvf command](./img-screenshots/g.archive-misc--tar.png)


8. `Compress the tar archive to create a misc.tar.gz file`
![gzip command](./img-screenshots/h.compress-misc.tar--misc.tar.gz.png)


9. `Create a user and force the user to change his/her password upon login`
![passwd -e command](./img-screenshots/i.new-user--nuel--ch-password-immediately.png)


10. `Lock a users password` `unlock user's password to ensure lock worked`
![passwd -l command](./img-screenshots/j.lock-unlock-nuel-password.png)


11. `Create a user with no login shell`
![no login shell](./img-screenshots/k.user-no-login-shell.png)


12. `Disable password based authentication for ssh`
![edit sshd_config file](./img-screenshots/l.disable-passwd-auth.png)    


13. `Disable root login for ssh`
![edit sshd_config file](./img-screenshots/m.disable-root-login.png)