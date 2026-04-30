---
title: "Functions (DAC Block: VBS-Driver)"
---

# Functions

28 functions from `Gfsvbsdr.chm`.

| Name | Summary |
| --- | --- |
| [`Append`](append.md) | Appends, in the Script driver, the contents of a variable (pvValue) to the pvBuffer output buffer in the vFormat . |
| [`Close`](close.md) | Closes an interface in the script driver that you opened with Open . |
| [`ErrorTextGet`](errortextget.md) | Calls an error description for the UDI device. |
| [`Open`](open.md) | Opens a communication channel to an interface in the script driver and initializes it with the current interface parameters. |
| [`ParamGet`](paramget.md) | Requests an interface-specific parameter from the UDI device in the script driver . |
| [`ParamSet`](paramset.md) | Sets an interface-specific parameter for the UDI device in the script driver . |
| [`Parse`](parse.md) | Accesses the data that DIAdem reads from a UDI device, using the Read command in the script driver . The function especially supports access to binary data. |
| [`Read`](read.md) | Reads data from the communication interface in the script driver . |
| [`SFD_DeInitInChannel`](sfd-deinitinchannel.md) | Deinitializes the inputs used in the script driver . DIAdem calls the SFD_DeInitInChannel function during the measurement wrap-up, once for every active measurement channel. |
| [`SFD_DeInitOutChannel`](sfd-deinitoutchannel.md) | Deinitializes an active output channel in the script driver . DIAdem calls the SFD_DeInitOutChannel function during the measurement wrap-up, once for every active output. |
| [`SFD_DeInitProcessChannel`](sfd-deinitprocesschannel.md) | Deinitializes the data processing channels used in the script driver . DIAdem calls the SFD_DeInitProcessChannel function during the measurement wrap-up, once for every active data processing channel. |
| [`SFD_DelInit`](sfd-delinit.md) | Deinitializes the connected devices and disconnects the devices in the script driver . DIAdem calls the SFD_DelInit function once during measurement follow-up tasks. |
| [`SFD_FinalInit`](sfd-finalinit.md) | Executes a final initialization of the connected device and the variables of the script in the script driver . DIAdem calls the SFD_FinalInit function once when it completes a measurement preparation. |
| [`SFD_FinalStop`](sfd-finalstop.md) | Ends the measurement or the communication with a device in the script driver . DIAdem calls the SFD_FinalStop function once when it completes the DAC task. |
| [`SFD_GetBlockScan`](sfd-getblockscan.md) | Requests in the Script driver several scans in the measurement mode Hardware clock from the connected device and saves the data in the specified variable field. |
| [`SFD_GetScan`](sfd-getscan.md) | Requests the measurement data of a complete scan from the connected device in the script driver and saves the data in the respective variables of the script. DIAdem calls the SFD_GetScan function once per measurement cycle. This function simplifies receiving data from a measurement device that always provides the data for a complete scan. |
| [`SFD_Init`](sfd-init.md) | Initializes the connection in the script driver and establishes the connection to the device. DIAdem calls the SFD_Init function once during a measurement preparation. |
| [`SFD_InitInChannel`](sfd-initinchannel.md) | Initializes the required measurement channels in the script driver . DIAdem calls the SFD_InitInChannel function during the measurement preparation, once for every active measurement channel. |
| [`SFD_InitOutChannel`](sfd-initoutchannel.md) | Initializes the required output channels in the script driver . DIAdem calls the SFD_InitOutChannel function during the measurement preparation, once for every active output. |
| [`SFD_InitProcessChannel`](sfd-initprocesschannel.md) | Initializes the required channels for data processing in the script driver . DIAdem calls the SFD_InitProcessChannel function during the measurement preparation, once for every active data processing channel. |
| [`SFD_ProcessChannel`](sfd-processchannel.md) | Offsets the data of the connected input signals against each other in the script driver . DIAdem calls this function once per measurement cycle for each channel in the block. |
| [`SFD_ProcessScan`](sfd-processscan.md) | Enables simultaneous processing of all signals of a scan in the script driver . You can save the results in a script global array, and then transfer the results to DIAdem with the SFD_ProcessChannel function. |
| [`SFD_ReadChannel`](sfd-readchannel.md) | Transfers the measurement data of a single channel from the script to the script driver . The function can request the data of this channel directly from the measurement device or from the respective script variables. Before the function can request measurement data from variables, the SFD_GetScan function must save the measurement data in variables, read out the data, and transfer the measurement data to the script driver. DIAdem calls this function once per measurement cycle for every active measurement channel. |
| [`SFD_SendScan`](sfd-sendscan.md) | Transfers the data of a complete scan to the connected device in the script driver . DIAdem calls this function once per measurement cycle. |
| [`SFD_Start`](sfd-start.md) | Restarts the measurement on the connected device when a trigger sequence changes in the script driver . |
| [`SFD_WriteChannel`](sfd-writechannel.md) | Transfers measured values from the script driver for output to the script. The function can transfer the measurement values either directly to the connected device or save the values in the respective variables of the script. If the function saves the measurement values in variables, the SFD_SendScan function can transfer the measurement values as a complete scan to the device. DIAdem calls this function once in each measurement cycle for each active output channel. |
| [`Sleep`](sleep.md) | Interrupts the script for a specified number of milliseconds in the script driver . |
| [`Write`](write.md) | Sends data to a connected device over a communication interface in the script driver . |
