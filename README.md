# TDC-based-Security-Primitive-with-Tunable-Parameters
-------------------------------------------------------


Description
-----------

This is a time-to-digital converter (TDC) based parameter-adjustable hardware security primitive that can be pre-deployed on FPGAs for trust evaluation, such as Hardware Trojans (HTs) detection.

The script IPGEN.py will import a pre-configuration file and then create the TDC-based IP core and the corresponding implementation constraints.
The pre-configuration file contains user-defined parameters that are referenced to adjust the TDC structure. 
These parameters include the instance name, the numbers of LUT and CARRY4 elements, respectively.
The measuring range of the TDC-based sensor is determined by the adjustment of the relative number of LUTs and CARRY4s.
The TDC-based IP core is specified in an Electronic Data Interchange Format (EDIF) netlist used as input to the Xilinx implementation tools.
The implementation constraints are exploited to maintain the instantiated order, in which relative location constraints are applied to the above groups of sensor elements. Using these files, the TDC-based hardware security primitive can be deployed on the FPGA platform without impacting the design under test.  

This TDC based security primitive is suitable for Xilinx Spartan-6 FPGAs. 


Package Structure
-----------------

This package contains the following files and folder:

-README 				: This file

-IPGEN			        : This folder contains IPGEN.py, configuration_file,txt and part1.txt for creating the TDC-based IP core.


Usage of the Security Primitive  
-------------------------------

You should integrate the security primitive into your design, including the TDC.edif and the TDC_ucf.ucf files from the IPGEN script.


Authors and Contact Details 
---------------------------

Haocheng Ma, 
hc_ma@tju.edu.cn,	
School of Microelectronics, Tianjin University, China

Jiaji He, 
jiaji_he@mail.tsinghua.edu.cn, 
Institute of Microelectronics, Tsinghua University, China


Copyright 
---------

It is mainly intended for non-commercial use, such as academic research.


Release Notes
------------

Build date : July 10, 2020
