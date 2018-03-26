# Custom Virtual Machine Size

## Requirements

Name     | Box                          | CPU | RAM | Disk   |
---------|------------------------------|-----|-----|--------|
ubuntu1  | ubuntu/xenial64              | 1   | 1GB | 10GB*  |
ubuntu2  | ubuntu/xenial64              | 1   | 1GB | 10GB*  |
ubuntu3  | ubuntu/xenial64              | 1   | 1GB | 10GB*  |
ubuntu4  | ubuntu/xenial64              | 1   | 1GB | 10GB*  |
freebsd5 | freebsd/FreeBSD-11.1-RELEASE | 1   | 1GB | 10GB*  |
freebsd6 | freebsd/FreeBSD-11.1-RELEASE | 1   | 1GB | 10GB*  |

## Setup and Start

One-liner:

```
mkdir ~/vm-imperialspeculate || cd ~/vm-imperialspeculate && curl -q https://raw.githubusercontent.com/stationgroup/vagrant-labs/master/imperialspeculate/Vagrantfile -O && vagrant up
```
