# Custom Virtual Machine Size

## Dependencies & Plugins

This _Vagrantfile_ needs the Vagrant plugin `vagrant-disksize` to resize the _box_ file with this variable: `config.disksize.size = "120GB"`

```
vagrant plugin install vagrant-disksize
```

## Requirements

Name    | Box             | CPU | RAM | Disk   |
--------|-----------------|-----|-----|--------|
ubuntu1 | ubuntu/xenial64 | 1   | 1GB | 10GB*  |
ubuntu2 | ubuntu/xenial64 | 1   | 4GB | 120GB* |
ubuntu3 | ubuntu/xenial64 | 1   | 1GB | 10GB*  |

###### _*Disk size shown is the maximum capacity. Disk grows with usage. ~1GB of disk space required per OS install._

## :floppy_disk: Setup and Start

One-liner:

```
mkdir ~/vm-offspringidea ; cd ~/vm-offspringidea && curl -q https://raw.githubusercontent.com/stationgroup/vagrant-labs/master/offspringidea/Vagrantfile -O && vagrant up
```
