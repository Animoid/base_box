## Build Your Own Boxes

First, install the following software:

* [Packer](http://packer.io)
* [Git](https://git-scm.com)
* [Vagrant](https://www.vagrantup.com)

Clone this project by

    git clone https://github.com/Animoid/base_box.git
    cd base_box

Inside the cloned project directory, a JSON file describes the box that can be built. You can use `packer build` to build the
box.

    packer build animoid_base_box.json

Congratulations! You now have an box file in the ./builds directory that can be added to Vagrant with the following command:

    vagrant box add builds/ubuntu-14.04.virtualbox.box --name animoid

The box should show up in Vagrant now:

```
$ vagrant box list
animoid (virtualbox, 0)
```
