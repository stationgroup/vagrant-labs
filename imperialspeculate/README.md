# Custom Virtual Machine Size

## Requirements

Name     | Box                          | CPU | RAM   | Disk   |
---------|------------------------------|-----|-------|--------|
ubuntu1  | ubuntu/xenial64              | 1   | 1GB   | 10GB*  |
ubuntu2  | ubuntu/xenial64              | 1   | 1GB   | 10GB*  |
ubuntu3  | ubuntu/xenial64              | 1   | 1GB   | 10GB*  |
ubuntu4  | ubuntu/xenial64              | 1   | 1GB   | 10GB*  |
freebsd5 | freebsd/FreeBSD-11.1-RELEASE | 1   | 512MB | 21GB*  |
freebsd6 | freebsd/FreeBSD-11.1-RELEASE | 1   | 512MB | 21GB*  |

###### _*Disk size shown is the maximum capacity. Disk grows with usage. ~1GB of disk space required per OS install._

## :floppy_disk: Setup and Start

One-liner:

```
mkdir ~/vm-imperialspeculate ; cd ~/vm-imperialspeculate && curl -q https://raw.githubusercontent.com/stationgroup/vagrant-labs/master/imperialspeculate/Vagrantfile -O && vagrant up
```

## Notes

### Errors on first boot of _freebsd5_ and _freebsd6_.

These vagrant boxes will error on first boot.

```
==> freebsd6: Mounting shared folders...
    freebsd6: /vagrant => /home/USER/vm-imperialspeculate
Vagrant is not able to mount VirtualBox shared folders on BSD-based
guests. BSD-based guests do not support the VirtualBox filesystem at
this time.

To change the type of the default synced folder, specify the type as
rsync or nfs:

    config.vm.synced_folder ".", "/vagrant", type: "nfs" # or "rsync"

Alternatively, if you do not need to mount the default synced folder,
you can also disable it entirely:

    config.vm.synced_folder ".", "/vagrant", disabled: true

You can read more about Vagrant's synced folder types and the various
configuration options on the Vagrant website.

This is not a bug in Vagrant.
```

Just run `vagrant up` again. You can still run `vagrant ssh freebsd5` to access the box.
