This repo contains examples of using [Vagrant by HashiCorp](https://www.vagrantup.com/) with [VirtualBox](https://www.virtualbox.org/).
Testing was carried out on host-PC with OS Windows 11 (or 10).

## Dependencies:
   - Vagrant version >= 2.4.0
   - VirtualBox version >= 7.0.14
   - host OS - Windows 11 (or 10)

## Recommendation
When using a host based on Windows OS, it is recommended to run the VirtualBox shell as an Administrator before using `Vagrantfile`.

## How to work
To use `Vagrantfile` and create VM, in the current directory run the comand:
     `vagrant up [vm_name]`
          [vm_name] - optional parameter, if use some VM's.
          By default (without parameters), `vagrant` up all VM's, discribed in Vagrantfile

To stop VM run the command:
     `vagrant halt [vm_name]`
          [vm_name] - optional parameter, if use some VM's.

To delete VM run the command:
     `vagrant destroy [vm-name] [-f]`
          [vm_name] - optional parameter, if use some VM's.
          By default (without parameters), `vagrant` up all VM's, discribed in Vagrantfile
          [-f] - optional parameter, forse destroy.

To connect to the VM via ssh, run the command:
     `vagrant ssh [vm-name]`
          [vm_name] - optional parameter, if use some VM's.

To connecting to via other terminals, use next createds:
          IP address:    127.0.0.1
          SSH port:      2222
          user:          vagrant
          password:      vagrant

To check Linux OS version in the VM, run the command:
     `hostnamectl`

To check IP address in the Linux VM, run the command:
     `hostname -I`



    *Distributed under [MIT license](https://github.com/k-and-v/Vagrant/blob/master/LICENSE). Permitted for free coping and free use.*