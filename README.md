# Cora Z7 Root Repository

## Cora Z7-07S XADC Demo

### Description

This branch contains sources for the Cora Z7-07S XADC Demo.

This project demonstrates how to use the Cora Z7-07S's ZYNQ FPGA's analog-to-digital core (referred to as the XADC) with a ZYNQ processor. Vivado is used to build the demo's hardware platform, and Vitis is used to program the bitstream onto the board and to build and deploy a C application.

To use this demo, the Cora Z7-07S must be connected to a computer over MicroUSB, which must be running a serial terminal.

A channel select index can be incremented by pressing button 0 and decremented by pressing button 1. The table below shows how the channel select index is used to select from the Cora's various analog inputs. RGB LED 0 is used to show the sign of the selected analog input. 
If the voltage read is greater than 0.5 Volts, the RGB LED is green; if the voltage read is less than -0.5 Volts, the RGB LED is red.

**Warning:** *Take care not to drive analog inputs below the Cora's ground or above 1.0V (for differential inputs) or above 3.3V (for single-ended inputs). Differential inputs operating in Bipolar mode provide negative readings when the negative input pin of the pair has a higher voltage than the positive, however, this does NOT imply that these inputs can safely be driven below the system ground.*

| Index     | Analog Input/s                           |
| --------- | ---------------------------------------- |
| 0         | VP/VN Dedicated Differential Input       |
| 1         | Shield Header A6-A7 Differential Input   |
| 2         | Shield Header A8-A9 Differential Input   |
| 3         | Shield Header A10-A11 Differential Input |
| 3         | Shield Header A0 Single-Ended Input      |
| 3         | Shield Header A1 Single-Ended Input      |
| 3         | Shield Header A2 Single-Ended Input      |
| 3         | Shield Header A3 Single-Ended Input      |
| 3         | Shield Header A4 Single-Ended Input      |
| 3         | Shield Header A5 Single-Ended Input      |

For more information on the Cora Z7-07S XADC Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/cora-z7/demos/xadc) on the Digilent Wiki.

For more information on the Cora Z7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cora-z7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Cora-Z7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes      |
| OS        | No       |
| SW        | Yes      |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Cora-Z7-07S-XADC/

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Cora Z7-07S
* MicroUSB cable
* Vivado and Vitis 2022.1 installations
* Serial Terminal Emulator
* Wires and a circuit to measure
