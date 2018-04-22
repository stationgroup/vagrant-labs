# Punkt.de FreeBSD Virtual Machine

## Dependencies & Plugins

This _Vagrantfile_ is from the German FreeBSD VPS [Punkt.de](https://punkt.de/en).

[vagrantup.com/punktde](https://app.vagrantup.com/punktde)

FreeBSD box we use for our internal development. Apart from FreeBSD 11 and the Vagrant environment it contains all the necessary packages to start with Ansible right away, but nothing more.

* Custom kernel with VIMAGE option (virtual network stack to use with jails).
* Packages: `sudo` `bash` `virtualbox-ose-additions` `python27` `python36`
* 60GB SCSI hdd with ZFS root

## Requirements

Name     | Box                     | CPU | RAM | Disk   |
---------|-------------------------|-----|-----|--------|
freebsd1 | punktde/freebsd-111-zfs | 1   | 1GB | 60GB*  |
freebsd2 | punktde/freebsd-111-zfs | 1   | 1GB | 60GB*  |
freebsd3 | punktde/freebsd-111-zfs | 1   | 1GB | 60GB*  |

###### _*Disk size shown is the maximum capacity. Disk grows with usage. ~1GB of disk space required per OS install._

## :floppy_disk: Setup and Start

One-liner:

```
mkdir ~/vm-candlemajor ; cd ~/vm-candlemajor && curl -q https://raw.githubusercontent.com/stationgroup/vagrant-labs/master/candlemajor/Vagrantfile -O && vagrant up
```
