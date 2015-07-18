# vagrant

Simple development environment for Vagrant used in [Harad](http://harad.mx).

**Table of Contents**

- [Requirements](#require)
- [Quickstart](#quickstart)
- [License](#license)


## <a name="require">Requirements</a>

1. You must have installed (Vagrant)[http://www.vagrantup.com/downloads.html]
2. And (VirtualBox)[https://www.virtualbox.org/wiki/Downloads]

## <a name="quickstart"></a>Quickstart

First at all clone our vagrant repository:

``` bash
$> mkdir harad
$> cd harad
$> git clone https://github.com/haradmx/vagrant.git vagrant
```

After that you can run your vagrant machine:

```
$ cd vagrant/
$ vagrant up --provision
```

Then the box will be downloaded for you.

If you wish, you can learn more about it alter a [vagrant file](Vagrantfile) and its [configuration options](ConfigOptions).

## <a name="license"></a>Copyright and license

***

Copyright (c) 2015 Iván Jaimes. See [LICENSE](LICENSE) for details.


[Vagrant]: http://www.vagrantup.com/
[Vagrantfile]: https://github.com/haradmx/vagrant/blob/master/Vagrantfile
[ConfigOptions]: http://docs.vagrantup.com/v2/vagrantfile/
