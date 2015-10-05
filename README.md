# CIAA Linux developer enviroment

This is a vagrant file that allows you to create a virtual box virtual machine based on ubuntu with an ARM compiler and OpenOCD already installed.

## Requirements

First of all you have to install:
- Virtualbox: https://www.virtualbox.org/wiki/Downloads
- Vagrant: https://www.vagrantup.com/downloads.html
- Git bash: https://git-scm.com

## Usage
Open a terminal console and type:

```
git clone https://github.com/ernesto-g/ciaa-vagrant.git
cd ciaa-vagrant
vagrant up --provider virtualbox
```

The first time vagrant will download the virtual machine image. Once the virtual machine is running, you can connect to it by SSH:

```
vagrant ssh
```

- User: vagrant
- Pass: vagrant
- sudo pass: vagrant

You can also use a common ssh client as PuTTY : http://www.putty.org


