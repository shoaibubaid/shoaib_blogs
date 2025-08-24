# ChipWhisperer Overview

ChipWhisperer is an open source tool chain that makes it easy to perform and analyse hardware attacks like side channel analysis and fault injection attacks.

The tool chain is basically of 4 components.

- ### Hardware
    This includes the devices that we have from ChipWhisperer, that is, 
    1. The scope (Lite board, Husky, pro, chipshouter) which captures the power or injects faults and,
    2. The Device under Test, i.e. the board where we are capturing the power from. These boards can be of STM32, XMEGA, esp32 etc.

    Usually, we already have these devices and their default state is enough for us. So we dont modify them much.

- ### Firmware
    This comprises of the firmware that we run on the hardware. This has the firmware for both the scope and DuT. But we mostly care about the firmware of DuT, i.e. the Micro controller we are interested in. So, this is an important part to understand because here is what we mainly modify the code.
- ### Software

    ChipWhisperer has its own python library to control the scope and communicate with the device under test. Even though we are not going to modify this code, we need to understand this properly to be able to use the APIs. There are 4 types of APIs by the way.

    1. scope API
    2. target API
    3. capture API
    4. analyzer API
- ### Tutorials
    Tutorials can be found in the jupyter section and do them as homework problems to understand APIs properly.


    --------------------------------------
    
    
# Jupyter Tutorials 

The sequence in which the tutorials should be followed is in this following way.

### Setting Up the System

<!-- * **[lab 1](#lab-1)**: Connecting to Hardware -->
* **[Lab 1](lab1/lab1.md)**: Connecting to Hardware

### SCA101: Introduction to Power Analysis Attacks

<!-- * **[Lab 2-1A](#lab-2-1a)**: Instruction Power Differences
* **[Lab 2-1B](#lab-2-1B)**: Power Analysis for Password Bypass -->
* **Lab 2-1A**: Instruction Power Differences
* **Lab 2-1B**: Power Analysis for Password Bypass
* **Lab 3-1**: Large hamming Weight Swings
* **Lab 3-2**: Recovering an AES Key from a Single Bit
* **Lab 3-3**: Recovery an AES key from a Power measurement (DPA)
* **Lab 4-1**: Showing the Hamming Weight relationship of data & power.
* **Lab 4-2**: Correlation Power Analysis
* **Lab 4-3**: Using ChipWhisperer for CPA Attacks
* **Lab 5-1**: ChipWhisperer CPA Attacks in Practice
* **Lab 6-4**: Triggering on UART

### SCA201: Power Analysis Attacks on AES Implementations
* **Lab 1-1A**: Resynchornizing Traces with Sum of Absolute Differences
* **Lab 1-1B**: Resynchornizing Traces with Dynamtic Time Warp
* **Lab 2-1**: CPA on a 32-bit AES Implementation
* **Lab 2-2**: CPA on a Hardware AES Implementation: Last-Round State
* **Lab 2-3**: CPA on a Hardware AES Implementation: Mix-Columns
* **Lab 3-1A**: AES-256 Bootloader Attack
* **Lab 3-B**: AES-256 Bootloader with Reverse Engineering using Power Analysis

### SCA202: Power Analysis on Asymmetric Implementations
* Power Analysis on 8-bit RSA Implementation (OLD VERSION IN REPO NOW)
* Power Analysis on MBED-TLS RSA Implementation (NOT IN REPO YET)
* Power Analysis on software ECC Implementation (NOT IN REPO YET)

### SCA203: Leakage Assesement
**NOTE: These labs are not here yet - but material is in the repo for some of this in sca203 folder**
* Introduction to Leakage Assessment
* Non-Specific TVLA on AES
* Specific TVLA on AES
* TVLA for Reverse Engineering
* TVLA on ECC

### SCA204: Power Analysis on Hardware ECC
* **Part 1**: Introduction to Hardware ECC Attacks
* **Part 2**: Improving the Attack
* **Part 3**: Countermeasures
* **Part 4**: More Countermeasures and Unintended Consequences
* **Part 5**: TVLA

### SCA205: Power Analysis on Software ECC
* **Part 1**: Breaking software ECC with TraceWhisperer
* **Part 2**: Breaking software ECC without TraceWhisperer
* **Part 3**: Breaking software ECC with TraceWhisperer *and* SAD

### FAULT101


* **Lab 1-1**: Introduction to Clock Glitching
* **Lab 1-2**: Clock Glitching to Bypass Password
* **Lab 1-3**: Clock Glitching to Dump Memory
* **Lab 1-4**: Authentication Bypass on AES Bootloader
* **Lab 2-1**: Introduction to Voltage Glitching
* **Lab 2-2**: Voltage Glitching to Bypass Password
* **Lab 2-3**: Voltage Glitching to Dump Memory

### FAULT201
* **Lab 1-1A**: Introduction to AES Fault Attacks
* **Lab 1-1B**: AES Loop Skip Fault Attack
* **Lab 1-2**: 1.5 Round AES Fault Attack
* **Lab 1-3A**: DFA Attack Against Final MixColumns
* **Lab 1-3B**: DFA Attack on AES
* **Lab 2-1**: Fault Attack on RSA


## Naming Notes

### Prefix

sca: Side Channel (Power) Analysis courses
fault: Fault Injection (Glitching) courses

### Numbering

* 1xx: Fundamentals. A 101 course is a prerequisite for all higher course.
* 2xx: Advanced topics. Dependencies noted in the labs/courses themselves.
* appx: Applications. Dependencies noted in the labs/courses themselves.

### Getting Started

We recommend going through sca101 before fault101, at least Lab 1_X and Lab 2_X. This will introduce you to the required ChipWhisperer software.

<!-- 
## My Section

This is the content of the section.

- [Go to My Section](#my-section)
- [Go to My Jupyter Tutorials](#jupyter-tutorials) -->

This is just to check if github actions are working or not!
This is just to check if github actions are working or not!

This is just to check if github actions are working or not!
