# DevOps - Vagrant 


## How to use these Labs
1. Install Vagrant: https://www.vagrantup.com/downloads.html

2. Install Oracle Virtual Box: https://www.virtualbox.org/wiki/Downloads

3. In a new Directory clone this respository:
``` shell
git clone https://github.com/thierno953/Vagrant.git
```
4. go into the lab folder corrasponding to the video you are watching. Example:
``` shell
cd get_started
```
5. Initialize the VM using vagrant init
``` shell
vagrant init bento/ubuntu-22.04
```
6. Bring up the vagrant instance

``` shell
vagrant up
```
7. Get Status of Local Vagrant Machine
``` shell
vagrant status
```

8. Get Status of Vagrant Machines on host
``` shell
vagrant global-status
```

9. Get SSH Settings
``` shell
vagrant ssh-config
```

10. Stop Virtual Machine
``` shell
vagrant reload
```

11. Stop Virtual Machine
``` shell
vagrant halt
```

12. Remove the Virtual Machine
``` shell
vagrant ssh
```