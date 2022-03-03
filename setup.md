---
layout: page
title: "Setup"
permalink: /setup/
---

# Transmitter

The transmitter consists of an LED, micro usb port, and antenna. 

Before plugging the Transmitter in, ensure the antenna is attached. Never supply power to the device without the antenna attached, as this can damage the radio module.

The LED is an indicator for the timer. Further explanation can be found [here](/starter_indicator_docs/transmitter).

# Remote

The remote consists of an LED, flip indicator, power switch, and micro usb port.

The micro USB port is used for charging. When fully charged, the device should last on battery for around 90 hours.

The device is off when the power switch is closest to the exterior, and on when the switch is closest to the micro USB port. When turning the device on, the LED should flash to indicate the device is on. Further explanation can be found [here](/starter_indicator_docs/remote).

# Computer

To operate, use a micro USB cable to connect the transmitter to the computer used for timing. The device should show up as a COM port in Windows Device Manager. Drivers will automatically install on Windows 10/11, you may need to install drivers manually if you are on Windows 7/8 - [Adafruit Feather Drivers](https://github.com/adafruit/Adafruit_Windows_Drivers/releases).

Download [simple_redlight.lss](simple_redlight.lss) to your system's Lynx directory.

Once you have the lss file copied and the device shows up in Device Manager, open FinishLynx and create a new scoreboard for the device. FinishLynx must be opened after the device is attached. If FinishLynx was running before attaching the device, you must close and reopen FinishLynx.

Scoreboard settings should use the COM port corresponding to the device as shown in Device Manager. 

Other settings are as follows (should be default):

```plaintext
Code Set: Single Byte

Serial Port: COM<#> (Modem)  Baud: 9600
Data Bits: 8  Parity: None  Stop Bits 1.0

Running Time: Normal  Options: <none should be checked>
Pause Time: 3.0  Offset: 0.000

Results: Off
```

