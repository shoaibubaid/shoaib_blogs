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

Start from the [Jupyter tutorials](jupyter/readme.md) and hopefully with each lab, we can learn new things incrementally.
