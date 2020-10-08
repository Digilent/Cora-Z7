# Cora Z7 Root Repository

## Cora Z7-07S Pmod-VGA Demo

### Description

This branch contains sources for the Cora Z7-07S Pmod-VGA Demo.

This project is a Vivado demo using the Cora Z7-07S's, Pmod Ports and the Pmod VGA written in VHDL. The Pmod VGA is controlled by the Cora Z7-07S through Pmod ports JA and JB. When programmed onto the board, a bouncing box and many test pattern bars are displayed on a connected VGA monitor. The screen resolution is configurable through HDL code.

You may want to change the display resolution if your VGA monitor does not support 1080p, or you want to modify the demo for a specific application. 
To select a different display resolution, select the appropriate set of Sync Generation constants for your target resolution from the list starting at line 47 of top.vhd. Uncomment the ten corresponding constants, FRAME_WIDTH through V_POL, and comment the default versions of those same constants. The default resolution is 1920×1080 @ 60Hz.

Next, select Project Manager in the Flow Navigator. In the Hierarchy tab of the Sources box, expand top under Design Sources and double click on clk_div_inst. Change the clk_out1 requested frequency to the required pxl_clk frequency specified in the selected resolution's Sync Generation comment block. 

For more information on the Cora Z7-07S Pmod-VGA Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/cora-z7/demos/pmod-vga) on the Digilent Wiki.

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
* https://github.com/Digilent/Cora-Z7-07S-Pmod-VGA/

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Cora Z7-07S
* MicroUSB cable
* Vivado 2020.1 installation
* Pmod VGA
* VGA Monitor
* VGA Cable