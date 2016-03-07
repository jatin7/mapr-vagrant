# MapR Base Vagrant Box
MapR v5.1.0 vagrant box including MapR FileSystem, MapR-DB and MapR Streams. This box is based on  [`puppetlabs/centos-6.6-64-nocm` box](https://atlas.hashicorp.com/puppetlabs/boxes/centos-6.6-64-nocm) and uses virtualbox as a provider.

Note: not for production use and only run this behind a firewalled internet connection.

## Box includes:
* MapR 5.1.0 (MapR FileSystem, MapR-DB and MapR Streams)

## Requirements
* [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/downloads.html)

## How to use the box
Start the MapR box:
```
vagrant init mkieboom/mapr-base
vagrant up
```

After that, point your internet browser towards the following url to start using MapR:
```
https://localhost:8443
Login: mapr
password: mapr
```

To ssh into the box use either one of the following:
```
vagrant ssh
or:
ssh -p 2222 <user>@localhost
```

where user can be any of the following:

## User credentials
Username/Password combinations on the box:
```
root/vagrant
vagrant/vagrant
mapr/mapr
```
## Register for FREE
Register your cluster for free by clicking the 'Register Now' button on the top of the MapR Control System Web UI to enable NFS and other unique MapR Features.

## Install other eco-system components
The vagrant box has been created using the MapR Installer. As such, you can use the same installer to add / remove eco-system components by simply pointing your internet browser to:
```
https://localhost:9443
Use mapr/mapr to login.
```