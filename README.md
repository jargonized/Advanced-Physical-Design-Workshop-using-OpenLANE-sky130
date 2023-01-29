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
|Fig. 1. Path to enter the working directory|

| ![files](labs/day1_2.png) | 
|:--:| 
|Fig. 2. Directory structure inside pdks|

| ![files](labs/day1_3.png) | 
|:--:| 
|Fig. 3. PDK(Process Design Kit) files for different process corners |

| ![files](labs/day1_4.png) | 
|:--:| 
|Fig. 4. Technology files for various open-source tools|

| ![files](labs/day1_5.png) | 
|:--:| 
|Fig. 5. Process specific files|

| ![files](labs/day1_6.png) | 
|:--:| 
|Fig. 6. Process specific Design Exchange Format (def) files|

| ![files](labs/day1_7.png) | 
|:--:| 
|Fig. 7. Openlane directory structure |

| ![files](labs/day1_8.png) | 
|:--:| 
|Fig. 8. Design files that come with the tool |

| ![files](labs/day1_9.png) | 
|:--:| 
|Fig. 9. config.tcl file - where all parameters are set - second highest priority |

| ![files](labs/day1_10.png) | 
|:--:| 
|Fig. 10. Contents of the file - design specific |

| ![files](labs/day1_11.png) | 
|:--:| 
|Fig. 11. Process Specific config.tcl file - highest priority for any design |

| ![files](labs/day1_12.png) | 
|:--:| 
|Fig. 12. Invoking OpenLANE and preparing the design |

| ![files](labs/day1_13.png) | 
|:--:| 
|Fig. 13. Notification of successful design preparation|

| ![files](labs/day1_14.png) | 
|:--:| 
|Fig. 14. Creation of runs folder - result of design prep|

| ![files](labs/day1_15.png) | 
|:--:| 
|Fig. 15. Directory Structure of 'runs' and 'tmp'|

| ![files](labs/day1_16.png) | 
|:--:| 
|Fig. 16. config.tcl file used by OpenLANE flow|

| ![files](labs/day1_17.png) | 
|:--:| 
|Fig. 17. Successful synthesis|

| ![files](labs/day1_18.png) | 
|:--:| 
|Fig. 18. Overall statistics of cells used|

| ![files](labs/day_19.png) | 
|:--:| 
|Fig. 19. Number of D- Flip Flops used|

| ![files](labs/day1_20.png) | 
|:--:| 
|Fig. 20. Area used by the module|

| ![files](labs/day1_21.png) | 
|:--:| 
|Fig. 21. Path to access Synthesis reports|

| ![files](labs/day1_22.png) | 
|:--:| 
|Fig. 22. Stat report - shown for example|

# 3. Day 2 - Good floorplan vs bad floorplan and Introduction to Library cells


| ![files](labs/day2_1.png) | 
|:--:| 
|Fig. 23. ASIC flow step-specific configuration files - default variable values assignment|

| ![files](labs/day2_2.png) | 
|:--:| 
|Fig. 24. Variable with descriptions and possible values|

| ![files](labs/day2_3.png) | 
|:--:| 
|Fig. 25. floorplan.tcl|

| ![files](labs/day2_4.png) | 
|:--:| 
|Fig. 26. Command to run floorplan|

| ![files](labs/day2_5.png) | 
|:--:| 
|Fig. 27. Successful completion of floorplan with the generation of PDN def|

| ![files](labs/day2_6.png) | 
|:--:| 
|Fig. 28. Floorplan log files|

| ![files](labs/day2_7.png) | 
|:--:| 
|Fig. 29. ioPlacer.log|

| ![files](labs/day2_8.png) | 
|:--:| 
|Fig. 30. Floorplan and PDN results|

| ![files](labs/day2_9.png) | 
|:--:| 
|Fig. 31. Path to access floorplan def file|

| ![files](labs/day2_10.png) | 
|:--:| 
|Fig. 32. Contents of floorplan.def file|

| ![files](labs/day2_11.png) | 
|:--:| 
|Fig. 33. Procedure to open the def file using magic - for visualisation|

| ![files](labs/day2_12.png) | 
|:--:| 
|Fig. 34. Layout zoomed to show equidistant IO pins|

| ![files](labs/day2_13.png) | 
|:--:| 
|Fig. 35. Selection of a horizontal IO pin|

| ![files](labs/day2_14.png) | 
|:--:| 
|Fig. 36. Viewing the metal layer|

| ![files](labs/day2_15.png) | 
|:--:| 
|Fig. 37. Selection of a vertical IO pin|

| ![files](labs/day2_16.png) | 
|:--:| 
|Fig. 38. Viewing the metal layer|

| ![files](labs/day2_17.png) | 
|:--:| 
|Fig. 39. Presence of tap and decap cells|

| ![files](labs/day2_18.png) | 
|:--:| 
|Fig. 40. Unplaced logic cells|

| ![files](labs/day2_19.png) | 
|:--:| 
|Fig. 41. Verifying the logic cells|

| ![files](labs/day2_20.png) | 
|:--:| 
|Fig. 42. Verifying the logic cells - contd.|

| ![files](labs/day2_21.png) | 
|:--:| 
|Fig. 43. Floorplan variable values that were used in the flow|

# 4. Day 3 - Design Library cells using magic layout and ngspice characterisation


| ![files](labs/day3_1.png) | 
|:--:| 
|Fig. 44. Dynamic assignment of variables|

| ![files](labs/day3_2.png) | 
|:--:| 
|Fig. 45. Change in IO pin placement|

| ![files](labs/day3_3.png) | 
|:--:| 
|Fig. 46. Magic command to open above layout - for reference|

| ![files](labs/day3_4.png) | 
|:--:| 
|Fig. 47. Cloning of vsdstdcelldesign repository|

| ![files](labs/day3_5.png) | 
|:--:| 
|Fig. 48. Contents of vsdstdcelldesign repo|

| ![files](labs/day3_6.png) | 
|:--:| 
|Fig. 49. Layout of inverter|

| ![files](labs/day3_7.png) | 
|:--:| 
|Fig. 50. Viewing the inference of the tool based on the layers used|

| ![files](labs/day3_8.png) | 
|:--:| 
|Fig. 51. Inference - contd.|

| ![files](labs/day3_9.png) | 
|:--:| 
|Fig. 52. Highlighting the metal contacts |

| ![files](labs/day3_10.png) | 
|:--:| 
| Fig. 53. Generated extracted spice file|

| ![files](labs/day3_11.png) | 
|:--:| 
| Fig. 54. Generated spice netlist |

| ![files](labs/day3_12.png) | 
|:--:| 
| Fig. 55. Netlist of inverter|

| ![files](labs/day3_13.png) | 
|:--:| 
| Fig. 56 Dimensions used by the magic tool|


| ![files](labs/day3_15.png) | 
|:--:| 
| Fig. 57. Contents of nshort.lib|

| ![files](labs/day3_16.png) | 
|:--:| 
| Fig. 58 Modified netlist to run simulation|

| ![files](labs/day3_17.png) | 
|:--:| 
| Fig. 59 Successful simulation|

| ![files](labs/day3_18.png) | 
|:--:| 
| Fig. 60 Plot of input and output pulse|

| ![files](labs/day3_19.png) | 
|:--:| 
| Fig. 61 Reduced spikes after increasing load capacitance|

| ![files](labs/day3_20.png) | 
|:--:| 
| Fig. 62 Rise time|

| ![files](labs/day3_21.png) | 
|:--:| 
| Fig. 63 Fall time|

| ![files](labs/day3_22.png) | 
|:--:| 
| Fig. 64 Rise propagation delay|

| ![files](labs/day3_23.png) | 
|:--:| 
| Fig. 65 Fall propagation delay|

| ![files](labs/day3_24.png) | 
|:--:| 
| Fig. 66 Test files for DRC |

| ![files](labs/day3_25.png) | 
|:--:| 
| Fig. 67 Contents of DRC config file, with local reference to sky130 technology file|

| ![files](labs/day3_26.png) | 
|:--:| 
| Fig. 68 Metal 3 layer magic file|

| ![files](labs/day3_27.png) | 
|:--:| 
| Fig. 69 DRC rule violation|

| ![files](labs/day3_28.png) | 
|:--:| 
| Fig. 70 Metal 3 Contact layer with CIF contact slots, satisfying the DRC rule automatically|

| ![files](labs/day3_30.png) | 
|:--:| 
| Fig. 71 Verification of distance values|

| ![files](labs/day3_31.png) | 
|:--:| 
| Fig. 72 Poly magic file|

| ![files](labs/day3_32.png) | 
|:--:| 
| Fig. 73 poly.9 rule defined by skywater pdk for 130nm process|

| ![files](labs/day3_33.png) | 
|:--:| 
| Fig. 74 Rule not satisfied, but no error shown thus pointing out the error in the drc file|

| ![files](labs/day3_34.png) | 
|:--:| 
| Fig. 75 Loading modified tech file|

# 5. Day 4 - Pre-layout timing analysis and importance of good clock tree


| ![files](labs/day4_1.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_2.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_3.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_4.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_5.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_6.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_7.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_8.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_9.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_10.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_11.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_12.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_13.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_14.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_15.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_16.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_17.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_18.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_19.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_20.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_21.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_22.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_23.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_24.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_25.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_26.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_27.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_28.png) | 
|:--:| 
| Fig.|

| ![files](labs/day4_29.png) | 
|:--:| 
| Fig.|


# 6. Day 5 - RTL2GDS using TritonRoute and OpenSTA

| ![files](labs/day5_1.png) | 
|:--:| 
| Fig.|

| ![files](labs/day5_2.png) | 
|:--:| 
| Fig.|

| ![files](labs/day5_3.png) | 
|:--:| 
| Fig.|

| ![files](labs/day5_4.png) | 
|:--:| 
| Fig.|

| ![files](labs/day5_5.png) | 
|:--:| 
| Fig.|

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
