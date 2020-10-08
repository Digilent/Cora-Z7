# Cora Z7 Root Repository

## Cora Z7-07S Basic-IO Demo

### Description

This branch contains sources for the Cora Z7-07S Basic-IO Demo.

This project is a Vivado demo using the Cora Z7-07S's RGB LED's and pushbuttons, written in Verilog. When programmed onto the board, the RGB LEDs will cycle from Blue to Green to Red to Black. As long as one of the two buttons is pushed, the corresponding RGB LED will be turned off.

For more information on the Cora Z7-07S Basic-IO Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/cora-z7/demos/basic-io) on the Digilent Wiki.

For more information on the Cora Z7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cora-z7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Cora-Z7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes      |
| OS        | No         |
| SW        | No         |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Cora-Z7-07S-Basic-IO/

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Cora Z7-07S
* MicroUSB cable
* Vivado 2020.1 installation