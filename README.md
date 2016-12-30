# nethserver-vagrant

### Description
Start a clean NethServer installation with [vagrant](https://www.vagrantup.com/)

### Prerequisites
 - VirtualBox / Libvirt / VMWare

 - Vagrant

 - Vagrantfile from this repo
```
Fedora
dnf install vagrant

Ubuntu \ Debian
apt-get install vagrant
```
### Start
- Set the IP of the virtual machine
- Set the interface name for the network bridge

`IPADDR=<ip_address> BRIDGE=<interface_name> vagrant up`

#### Example

If your interface name is `enp2s0` and the IP of the machine will be `192.168.5.228` the command is:

`IPADDR=192.168.5.228 BRIDGE=enp2s0 vagrant up`

At the end of the installation you can easily SSH into machine with

`vagrant ssh` or `ssh root@<ip_address>`