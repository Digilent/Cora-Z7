# Cora Z7 Root Repository

## Cora Z7-10 Petalinux Demo

### Description

This branch contains sources for the Cora Z7-10 Petalinux Demo.

The project includes the following features by default:

* Ethernet with Unique MAC address and DHCP support (see known issues)
* USB Host support
* UIO drivers for onboard buttons and LEDs
* SSH server
* Build essentials package group for on-board compilation using gcc, etc. 
* U-boot environment variables can be overriden during SD boot by including uEnv.txt in the root directory of the SD card (see u-boot documentation).

For more information on the Cora Z7-10 Petalinux Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/cora-z7/demos/petalinux) on the Digilent Wiki.

For more information on the Cora Z7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cora-z7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Cora-Z7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes         |
| OS        | Yes         |
| SW        | No         |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Cora-Z7-10-base-linux and https://github.com/Digilent/Petalinux-Cora-Z7-10

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Cora Z7-10
* MicroUSB Cable
* Vivado 2020.1 and Petalinux 2020.1 installations
* microSD card