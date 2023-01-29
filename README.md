# Advanced Physical Design Workshop using OpenLANE sky130

![Workshop Banner](/docs/poster.png)

# About

A cloud based 5 day training workshop which offered insights into design and characterization standard cell, and a hands-on in the Physical Design Domain (RTL to GDSII) using OpenLANE as the EDA tool and sky130 as the PDK.

Workshop conducted by VLSI System Design : [VSD website](https://www.vlsisystemdesign.com/)

# Outline

1. [Introduction](#1-introduction)
2. [Day 1 - Inception of open-source EDA, OpenLANE and sky130 PDK](#2-day-1---inception-of-open-source-eda-openlane-and-sky130-pdk) 
3. [Day 2 - Good floorplan vs bad floorplan and Introduction to Library cells](#3-day-2---good-floorplan-vs-bad-floorplan-and-introduction-to-library-cells)
4. [Day 3 - Design Library cells using magic layout and ngspice characterisation](#4-day-3---design-library-cells-using-magic-layout-and-ngspice-characterisation)
5. [Day 4 - Pre-layout timing analysis and importance of good clock tree](#5-day-4---pre-layout-timing-analysis-and-importance-of-good-clock-tree)
6. [Day 5 - RTL2GDS using TritonRoute and OpenSTA](#6-day-5---rtl2gds-using-tritonroute-and-opensta)
7. [Summary](#7-summary)
8. [Acknowledgement](#8-acknowledgement)
9. [Bibliography](#9-bibliography)

# 1. Introduction

# 2. Day 1 - Inception of open-source EDA, OpenLANE and sky130 PDK

| ![files](labs/day1_1.png) | 
|:--:| 
|Fig 1. Path to enter the working directory|

| ![files](labs/day1_2.png) | 
|:--:| 
|Fig 2. Directory structure inside pdks|

| ![files](labs/day1_3.png) | 
|:--:| 
|Fig 3. PDK(Process Design Kit) files for different process corners |

| ![files](labs/day1_4.png) | 
|:--:| 
|Fig 4. Technology files for various open-source tools|

| ![files](labs/day1_5.png) | 
|:--:| 
|Fig 5. Process specific files|

| ![files](labs/day1_6.png) | 
|:--:| 
|Fig 6. Process specific Design Exchange Format (def) files|

| ![files](labs/day1_7.png) | 
|:--:| 
|Fig 7. Openlane directory structure |

| ![files](labs/day1_8.png) | 
|:--:| 
|Fig 8. Design files that come with the tool |

| ![files](labs/day1_9.png) | 
|:--:| 
|Fig 9. config.tcl file - where all parameters are set - second highest priority |

| ![files](labs/day1_10.png) | 
|:--:| 
|Fig 10. Contents of the file - design specific |

| ![files](labs/day1_11.png) | 
|:--:| 
|Fig 11. Process Specific config.tcl file - highest priority for any design |

| ![files](labs/day1_12.png) | 
|:--:| 
|Fig 12. Invoking OpenLANE and preparing the design |

| ![files](labs/day1_13.png) | 
|:--:| 
|Fig 13. Notification of successful design preparation|

| ![files](labs/day1_14.png) | 
|:--:| 
|Fig 14. Creation of runs folder - result of design prep|

| ![files](labs/day1_15.png) | 
|:--:| 
|Fig 15. Directory Structure of 'runs' and 'tmp'|

| ![files](labs/day1_16.png) | 
|:--:| 
|Fig 16. config.tcl file used by OpenLANE flow|

| ![files](labs/day1_17.png) | 
|:--:| 
|Fig 17. Successful synthesis|

| ![files](labs/day1_18.png) | 
|:--:| 
|Fig 18. Overall statistics of cells used|

| ![files](labs/day_19.png) | 
|:--:| 
|Fig 19. Number of D- Flip Flops used|

| ![files](labs/day1_20.png) | 
|:--:| 
|Fig 20. Area used by the module|

| ![files](labs/day1_21.png) | 
|:--:| 
|Fig 21. Path to access Synthesis reports|

| ![files](labs/day1_22.png) | 
|:--:| 
|Fig 22. Stat report - shown for example|

# 3. Day 2 - Good floorplan vs bad floorplan and Introduction to Library cells


| ![files](labs/day2_1.png) | 
|:--:| 
|Fig 23. |

| ![files](labs/day2_2.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_3.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_4.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_5.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_6.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_7.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_8.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_9.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_10.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_11.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_12.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_13.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_14.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_15.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_16.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_17.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_18.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_19.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_20.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day2_21.png) | 
|:--:| 
| Files used throughout the course|

# 4. Day 3 - Design Library cells using magic layout and ngspice characterisation


| ![files](labs/day3_1.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_2.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_3.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_4.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_5.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_6.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_7.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_8.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_9.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_10.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_11.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_12.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_13.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_14.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_15.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_16.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_17.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_18.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_19.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_20.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_21.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_22.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_23.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_24.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_25.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_26.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_27.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_28.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_29.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_30.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_31.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_32.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_33.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day3_34.png) | 
|:--:| 
| Files used throughout the course|

# 5. Day 4 - Pre-layout timing analysis and importance of good clock tree


| ![files](labs/day4_1.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_2.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_3.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_4.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_5.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_6.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_7.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_8.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_9.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_10.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_11.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_12.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_13.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_14.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_15.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_16.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_17.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_18.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_19.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_20.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_21.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_22.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_23.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_24.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_25.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_26.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_27.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_28.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day4_29.png) | 
|:--:| 
| Files used throughout the course|


# 6. Day 5 - RTL2GDS using TritonRoute and OpenSTA

| ![files](labs/day5_1.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day5_2.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day5_3.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day5_4.png) | 
|:--:| 
| Files used throughout the course|

| ![files](labs/day5_5.png) | 
|:--:| 
| Files used throughout the course|

# 7. Summary

The outcomes of this workshop are as follows:
 - How to talk to computers
 - SoC design and OpenLANE
 - Starting RISC-V SoC Reference design
 - Get familiar to open-source EDA tools
 - Chip Floor planning considerations
 - Library Binding and Placement
 - Cell design and characterization flows
 - General timing characterization parameters
 - Labs for CMOS inverter ngspice simulations
 - Inception of Layout – CMOS fabrication process
 - Sky130 Tech File Labs
 - Timing modelling using delay tables
 - Timing analysis with ideal clocks using openSTA
 - Clock tree synthesis TritonCTS and signal integrity
 - Timing analysis with real clocks using openSTA
 - Routing and design rule check (DRC)
 - PnR interactive flow tutorial

# 8. Acknowledgement

The above work was carried out as a part of the 5-day workshop on Advanced Physical Design organised by VLSI System Design. I am greatly indebted to Kunal Ghosh (course instructor), Timothy Edwards (Guest Instructor), Mohammed Shalan (Guest Instructor), Nickson Jose, efabless and the entire VSD Team for this great learning experience and immense guidance provided throughout the workshop.

# 9. Bibliography


Revision notes: Only lab screenshots uploaded.
