# Example High Speed CSV data logger

## Disclaimer
This is a personal guide not a peer reviewed journal or a sponsored publication. We make
no representations as to accuracy, completeness, correctness, suitability, or validity of any
information and will not be liable for any errors, omissions, or delays in this information or any
losses injuries, or damages arising from its display or use. All information is provided on an as
is basis. It is the reader’s responsibility to verify their own facts.

The views and opinions expressed in this guide are those of the authors and do not
necessarily reflect the official policy or position of any other agency, organization, employer or
company. Assumptions made in the analysis are not reflective of the position of any entity
other than the author(s) and, since we are critically thinking human beings, these views are
always subject to change, revision, and rethinking at any time. Please do not hold us to them
in perpetuity.

## Overview 
Demo of high speed logging to CSV.  

### Performance overview
IPC | Performance Class | AddBool | AddBoolLiteral | AddInt | AddIntLiteral | AddString "test" | AddStringLiteral "test" | Max buffer size (Write 10000 records of 8 x int, task @ 1ms)
-|-|-|-|-|-|-|-|-
Laptop | 93 | 0.8us | 0.4us | 0.3us | 0.3us | 0.6us | 0.3us | 
CX5140 | 50 | 2.0us | 1.1us | 1.1us | 0.9us | 1.3us | 1.0us | 6453 Bytes
C6015 2 Core| 40 | 2.2us | 1.1us | 1.3us | 1.0us | 1.4us | 1.3us | 3100 Bytes
CX8190 | 20 | tba | tba | tba | tba | tba | tba | 4650 Bytes

## Install 
Not required.  Simply open the project.

## TwinCAT
This project uses TcXaeShell 3.1.4024.10

## Getting started
This is not a guide for TcXaeShell, please visit http://beckhoff.com/ for further guides
* Open the included TwinCAT project and activate on your local machine
* Login and set the PLC running
* Open the HMI in live view

