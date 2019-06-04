# High-Level Synthesis Flow on Zynq using Vivado HLS

This course provides users with an understanding of high-level synthesis design methodologies necessary to develop digital systems using Vivado HLS 2018.2 version.

The labs have been developed on a PC running Microsoft Windows 10 professional edition and using **Vivado 2018.2** version tools.These labs can also be run using WebPack edition.

## Source Files Setup

To use the source files for each of the labs in this workshop, you have to clone this repository from Github. For that, do the following:

  If in **Windows**, download [Cmder](http://cmder.net/) or download [Git Bash](https://git-scm.com/download/win)

  If in **Ubuntu (or any Debian distribution)**, install git from the aptitude package manager by running this command in a terminal window:
  ```
  sudo apt-get install git
  ```

  After installing, set up git from [here](https://help.github.com/articles/set-up-git/).  Then open a new git-bash/cmder/terminal window and run the following command:
  ```
  git clone https://github.com/xupgit/High-Level-Syntheis-Flow-o-Zynq-using-Vivado-HLS.git
  ```

**Either copy the _source_ directory into _labs_ directory OR rename the _source_ directory as the _labs_**

In the instructions for the labs;

**{sources}** refers to the location where you will get the base files for the labs [here](https://github.com/xupgit/High-Level-Syntheis-Flow-on-Zynq-using-Vivado-HLS/tree/master/source)

**{labs}** refers to the location which you will use as your workspace for the labs in the workshop

**{boards}** refers to the target board, currently, PYNQ-Z1 and PYNQ-Z2 are the supported target boards

---
**NOTE**

Board support for the PYNQ-Z1 and PYNQ-Z2 are not included in Vivado 2018.2 by default. The relevant files need to be extracted and saved to:

 {Vivado installation}\data\boards\board_files\zynq

These files can be downloaded from [/board_files](https://github.com/xupgit/Zynq-Design-using-Vivado/tree/master/board_files).

---

## Hardware Setup

**PYNQ-Z2**:  Connect the board to the PC using a micro USB cable. Make sure that a jumper is connected to JTAG (between JP1\_1 and JP1\_2) to use the board in the development mode.  Also, make sure that another jumper is placed between J9\_2 and J9\_3 to select USB as a power source.


**PYNQ-Z1**:  Connect the board to the PC using a micro USB cable. Make sure that a jumper is connected to JTAG (between JP4\_1 and JP4\_2) to use the board in the development mode.  Also, make sure that another jumper is placed between JP5\_2 and JP5\_3 to select USB as a power source.

---

## Labs Overview

### Lab1:

This lab provides a basic introduction to high-level synthesis using the Vivado HLS tool flow. You will use
Vivado HLS in GUI mode to create a project. You will simulate, synthesize, perfrom design analysis, and implement the provided
model.

### Lab2:

This lab introduces various techniques and directives which can be used in Vivado HLS to improve
design performance. The design under consideration accepts an image in a (custom) RGB format,
converts it to the Y’UV color space, applies a filter to the Y’UV image and converts it back to RGB.

### Lab3:

This lab introduces various techniques and directives which can be used in Vivado HLS to improve
design performance as well as area and resource utilization. The design under consideration performs
discrete cosine transformation (DCT) on an 8x8 block of data.

### Lab4:

This lab introduces a design flow to generate a IP-XACT adapter from a design using Vivado HLS and
using the generated IP-XACT adapter in a processor system using IP Integrator in Vivado.

**Note.** Since PYNQ-Z1 board does not have Audio CODEC chip, this lab cannot be ported/verfied on the PYNQ-Z1 board, though design flow is still applicable to the board.
