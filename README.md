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

### Change VM's IP
Editing Vagrantfile in line 30, you can change dhcp mode by static ip address mode. Then you will be able to use any ssh client specifying a known ip address.

```
 # config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.network "private_network", type: "dhcp"
```  
You need to restart vagrant VM using the commad:
```
vagrant reload
```

