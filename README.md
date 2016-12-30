# nethserver-vagrant

### Description
Start a clean NethServer installation with [vagrant](https://www.vagrantup.com/)

### Prerequisites
 - VirtualBox / Libvirt / VMWare

 - Vagrant
```
Fedora
dnf install vagrant

Ubuntu \ Debian
apt-get install vagrant
```
 - Vagrantfile from this repo

### Start
- Set the IP of the virtual machine
- Set the interface name for the network bridge

`IPADDR=<ip_address> BRIDGE=<interface_name> vagrant up --provider <your_vm_provider>`

#### Example

- Interface name: `enp2s0`
- IP: `192.168.5.228`
- Provider: `virtualbox`

the command is:


`IPADDR=192.168.5.228 BRIDGE=enp2s0 vagrant up --provider virtualbox`

### SSH Access
You can easily SSH into machine with

`vagrant ssh` or `ssh root@<ip_address>`

default credentials are:
- username: `root`
- password: `vagrant`