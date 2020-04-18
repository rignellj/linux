# linux
This repository contains virtual box installation, ssh remote access using valgrind in linux and related stuff

## 1
Installation

```
su root
apt install sudo
sudo apt update
sudo apt upgrade
```

## 2
Setting up nonroot user:


`sudo adduser <login>` 
-> asks information about user
`sudo adduser <login> sudo`
-> give sudo privilages to <login>


## 3
Install commands: make, gcc, ssh

```
sudo apt-get install ssh
sudo /etc/init.d/ssh restart
sudo apt-get install gcc
sudo apt-get install make
```

## 4
Create SSH-key for host user:


`ssh-keygen -t rsa`
`scp -P <portnumber> .ssh/id_rsa.pub username@***.***.***.***:~/.ssh/authorized_keys2` -> to copy the public key file to your remote computer.
`scp -rP <portnumber> ~/ft_ls/ username@***.***.***.***:~/` -> to copy your files/directories into your virtual machine

## 5
Install Valgrind in your Linux machine

```
sudo apt-get install valgrind
```

## 6
Connect VSCode via SSH-key

```
ssh username@***.***.***.*** -p <portnumber>
```


# Voilà
