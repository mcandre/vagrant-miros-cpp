# vagrant-miros-cpp: a Vagrant box for building C/C++ binaries for MirOS (MirBSD)

(A placeholder for gcc, which comes with the gnu10.ngz distribution package.)

# VAGRANT CLOUD

* https://app.vagrantup.com/mcandre/boxes/vagrant-miros-cpp-i386

# EXAMPLE

```console
$ cd i386/test
$ vagrant up
$ vagrant ssh -c "cd /vagrant && g++ -o hello hello.cpp && ./hello"
Hello World!
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

## Recommended

* [vagrant-rsync-back](https://github.com/smerrill/vagrant-rsync-back) assists in copying artifacts from the guest to the host

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ sh -c "cd i386 && make vagrant-miros-cpp-i386.box"
```
