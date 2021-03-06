# Vagrant Laboratory
:neckbeard: Simple declarative mutable infrastructure laboratory.

# Install Vagrant and Virtualbox

## :floppy_disk: macOS

```
brew cask install virtualbox vagrant
```

## :floppy_disk: Linux (Ubuntu)

```
sudo apt -y install virtualbox vagrant
```

---

### [`imperialspeculate`](https://github.com/stationgroup/vagrant-labs/tree/master/imperialspeculate)

Name     | Box                          | CPU | RAM   | Disk   |
---------|------------------------------|-----|-------|--------|
ubuntu1  | ubuntu/xenial64              | 1   | 1GB   | 10GB*  |
ubuntu2  | ubuntu/xenial64              | 1   | 1GB   | 10GB*  |
ubuntu3  | ubuntu/bionic64              | 1   | 1GB   | 10GB*  |
ubuntu4  | ubuntu/bionic64              | 1   | 1GB   | 10GB*  |
freebsd5 | freebsd/FreeBSD-11.1-RELEASE | 1   | 512MB | 21GB*  |
freebsd6 | freebsd/FreeBSD-11.1-RELEASE | 1   | 512MB | 21GB*  |

---

### [`offspringidea`](https://github.com/stationgroup/vagrant-labs/tree/master/offspringidea)

Name    | Box             | CPU | RAM | Disk   |
--------|-----------------|-----|-----|--------|
ubuntu1 | ubuntu/xenial64 | 1   | 1GB | 10GB*  |
ubuntu2 | ubuntu/xenial64 | 1   | 4GB | 120GB* |
ubuntu3 | ubuntu/bionic64 | 1   | 1GB | 10GB*  |

---
###### _*Disk size shown is the maximum capacity. Disk grows with usage. ~1GB of disk space required per OS install._
