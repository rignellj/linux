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

```
sudo adduser <login> -> asks information about user
sudo adduser <login> sudo -> give sudo privilages
```

## 3
Install commands: make, gcc, ssh

```
sudo apt-get install ssh
systemctl restart ssh
sudo apt-get install gcc
sudo apt-get install make
```

## 4
Create SSH-key for host user:

```
ssh-keygen -t rsa

