Goodix touchscreen Linux driver
-------------------------------

See source code for actual device support.

This repository was used for driver development when the driver was
still out-of-tree. The repository is however still updated with the
latest upstream patches, to make it easier to experiment and review
changes.

New features, and bug reports should be made using the usual kernel
development process, through the linux-input@ mailing-list.

The code is under the same license as the Linux kernel itself. See
COPYING file for details.

Installing the Goodix Touchscreen
```sh
sudo apt-get install build-essential linux-headers-generic git   (skip this if you have already done it above)
git clone https://github.com/hadess/gt9xx.git
cd gt9xx
make
sudo make install
sudo depmod -a
sudo modprobe goodix_backport
```
