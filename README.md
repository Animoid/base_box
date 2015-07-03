## Build Your Own Boxes

First, install the following software:

* [Packer](http://packer.io)
* [Git](https://git-scm.com)

Clone this project with ```git clone https://github.com/Animoid/base_box.git```

Inside the cloned project directory, a JSON file describes the box that can be built. You can use `packer build` to build the
box.

    $ packer build animoid_base_box.json

Congratulations! You now have an box file in the ../builds directory that you can then add to Vagrant and start testing with.
