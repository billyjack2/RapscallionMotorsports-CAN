# CAN Definitions for RaceStudio3

## Ford Boss 302R ABS
To be used with the Ford Boss 302R ABS Module. This protocol is not complete, and only the following are supported:
Wheel Speeds 
Brake Pressure - Pressure is not completely correct, but can be used as a reference

Wheel speeds read 344 Mph if there is a wheel speed error. 
If there is more interest, I may spend more work on this. 

## Haltech - TurboLamik
Combines Haltech ECU Protocol with TurboLamik TCU Protocol
The TurboLamik should be configured to output CAN on ID 704 in TunerPro - 0x2C0. 
0x2C0 and 0x2C1 are expansion modules in Haltech's NSP software and can be configured to use up to 8 signals.
0x2C0 and 0x2C1 are not defined in the protocol since they will be defined in NSP and communicated via ECU parameters.

## Installation Instructions
1. Click on the desired file
2. Click download raw file on the right
3. Save in any location on your machine
4. In RaceStudio, click the 7th logo from the left - CAN protocols
5. Click import, "AiM protocol file", and locate the downloaded file.
6. In the configuration you are using, select the appropriate CAN stream
7. Click the Protocol drop-down and select the imported protocol
