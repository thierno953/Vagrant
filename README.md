# DevOps - Vagrant Labs


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
6. Run the vagrant up command

``` shell
vagrant up
```
7. SSH into the VM

``` shell
vagrant ssh
```