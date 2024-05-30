# Haltech - TurboLamik
Combines Haltech ECU Protocol with TurboLamik TCU Protocol and includes values not supported by the AiM default protocol. This will also be updated as Haltech and Turbolamik update their protocols.


The TurboLamik should be configured to output CAN on ID 704 in TunerPro - 0x2C0. 

0x2C0 and 0x2C1 are expansion modules in Haltech's NSP software and can be configured to use up to 8 signals.

0x2C0 and 0x2C1 are not defined in the protocol since they will be defined in NSP and communicated via ECU parameters.


## TunerPro Setup - TODO

## Protocol Supported Values
> [!NOTE]
> Not all Haltech values are supported. This will be expanded over time. Feel free to request missing values you would like to see.

| ID | Name | Description | Unit |
| ---- | ---- | ----------- | ---- |
| CC01 | TCU Gear | TCU Gear Request | R-8 |
| CC02 | TCU Oil Temp | 8HP oil temp | F |
| CC03 | TCU Prog Sw | TCU Current Prog | 1-8 |
| CC04 | TCU Error | TCU Error Code | Link |
| CC05 | TCU TQ Red | Torque Reduction Request | Bool |
| CC06 | TCU Safety Mode | | bool |
| CC07 | TCU Park Act | Park Activated | bool |
| CC08 | TCU Oil Fan Rq | Oil fan request | bool |
| CC09 | TCU TranBrake | Transmission Brake active | bool |
| CC10 | TCU Auto Mode | | bool |
| CC11 | TCU Brk Solen On | Brake Solenoid On | bool |
