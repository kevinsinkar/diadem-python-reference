---
title: "Commands (Commands - Online (DAC))"
---

# Commands

246 commands from `ComOnl.chm`.

| Name | Summary |
| --- | --- |
| [`ADMAdmin`](admadmin.md) | Opens the dialog box for user management. If the user is not logged on in the user management, DIAdem opens the dialog box for logging on. |
| [`ADMCreateRight`](admcreateright.md) | Creates a new access right for the user management. |
| [`ADMLogin`](admlogin.md) | Opens the user management dialog box where the user logs on and off. |
| [`ADMLogout`](admlogout.md) | Logs out the current user from the user management. |
| [`AskADMPermission`](askadmpermission.md) | Checks the access rights of the current user and opens the dialog box for logging on if the user does not have the required rights. |
| [`AskADMPermRt`](askadmpermrt.md) | Checks the access rights of the current user. |
| [`BlCopy`](blcopy.md) | Duplicates a DAC block in the current block diagram. |
| [`BlDel`](bldel.md) | Deletes a DAC block in the current block diagram. |
| [`BlObjNew`](blobjnew.md) | Creates a new DAC block in the current block diagram. |
| [`BlPinCableInit`](blpincableinit.md) | Opens the dialog box where you connect buses to a DAC block. |
| [`BlPinDel`](blpindel.md) | Delete signal connections in sub-block diagrams. |
| [`BlPinNew`](blpinnew.md) | Creates a new block terminal in subblock diagrams. |
| [`BlPinSigCountSet`](blpinsigcountset.md) | Specifies the number of terminals at inputs and outputs on DAC blocks and subblock diagrams. |
| [`BlPinSigNameGen`](blpinsignamegen.md) | Overwrites in terminals of blocks and subblock diagrams the terminal names with the signal names. |
| [`BlReplace`](blreplace.md) | Replaces a DAC block with another similar DAC block in the current block diagram. |
| [`DACColorInit`](daccolorinit.md) | Displays a block diagram in the default colors. |
| [`DACEditLock`](daceditlock.md) | Locks the configuration of a block diagram or unlocks it. |
| [`DACFontInit`](dacfontinit.md) | Redisplays a block diagram in the default font. |
| [`DACObjClose`](dacobjclose.md) | Closes a DAC block after the configuration. |
| [`DACObjDestroy`](dacobjdestroy.md) | Cancels access to a DAC object without adopting a configuration. |
| [`DACObjDlg`](dacobjdlg.md) | Specifies the dialog box title of a DAC block. |
| [`DACObjOpen`](dacobjopen.md) | Opens a DAC object to set the parameters for the object. |
| [`DACObjPosSet`](dacobjposset.md) | Positions a DAC block in the block diagram. |
| [`DACObjRename`](dacobjrename.md) | Assigns a new block name to the DAC block in the loaded block diagram. |
| [`DACObjWhere`](dacobjwhere.md) | Searches for DAC blocks in the current block diagram. |
| [`DCSConvertBinToPhys`](dcsconvertbintophys.md) | Uses a type description to convert a binary number into the physical value. |
| [`DCSConvertDTCToString`](dcsconvertdtctostring.md) | Converts a 2-byte diagnostic trouble code (DTC) into a string in compliance with SAE J2012. |
| [`DCSConvertPhysToBin`](dcsconvertphystobin.md) | Uses a type description to convert a physical value into a binary number. |
| [`DCSDataRead`](dcsdataread.md) | Uses a local identifier to read data from the engine control unit (ECU). |
| [`DCSDataToString`](dcsdatatostring.md) | Converts the read data into a string. |
| [`DCSDataWrite`](dcsdatawrite.md) | Uses a local identifier to write data onto the engine control unit (ECU). |
| [`DCSDiagnosticClose`](dcsdiagnosticclose.md) | Finishes a diagnosis. |
| [`DCSDiagnosticFrameSend`](dcsdiagnosticframesend.md) | Uses a diagnostics-CAN-ID to send a CAN frame to the engine control unit (ECU), in order to check the transport log for errors. |
| [`DCSDiagnosticServiceExecute`](dcsdiagnosticserviceexecute.md) | Executes a diagnosis service. If a specific service from the KWP2000-, UDS- or OBD-service function are not available, you can use this function to call the respective service. |
| [`DCSDiagnosticSessionStart`](dcsdiagnosticsessionstart.md) | Starts a diagnosis and sets the engine control unit (ECU) into diagnostic mode. |
| [`DCSDiagnosticSessionStop`](dcsdiagnosticsessionstop.md) | Ends a diagnosis and resets the engine control unit (ECU) to normal mode. |
| [`DCSDiagosticFrameReceive`](dcsdiagosticframereceive.md) | Uses a diagnostics-CAN-ID to receive a CAN frame, in order to check the transport log for errors. |
| [`DCSDoIPConnect`](dcsdoipconnect.md) | Generates a TCP/IP connection to a DoIP unit through the IP address. |
| [`DCSDoIPDisconnect`](dcsdoipdisconnect.md) | Separates the TCP/IP connection to a DoIP unit. |
| [`DCSDoIPEntitiesGet`](dcsdoipentitiesget.md) | Specifies a table with the DoIP units (vehicles) of the local sub-net which refers to the entity ID (EID) or the vehicle ID number (VIN). |
| [`DCSDoIPEntityAddress`](dcsdoipentityaddress.md) | Specifies the address of one of the DoIP units in the list. |
| [`DCSDoIPEntityEntityID`](dcsdoipentityentityid.md) | Specifies the entity ID (EID) of one of the DoIP units in the list. |
| [`DCSDoIPEntityGroupID`](dcsdoipentitygroupid.md) | Specifies the group ID of an element from DoIP units in a list. |
| [`DCSDoIPEntityIPAddress`](dcsdoipentityipaddress.md) | Specifies the IP address of an element from DoIP units in a list. |
| [`DCSDoIPEntityListSize`](dcsdoipentitylistsize.md) | Specifies the length of the list with DoIP units. |
| [`DCSDoIPEntityPowerStateGet`](dcsdoipentitypowerstateget.md) | Specifies the diagnosis status of a DoIP unit. |
| [`DCSDoIPEntityStatusCurrentSockets`](dcsdoipentitystatuscurrentsockets.md) | Determines the number of currently established TCP/IP sockets from the DCSDoIPEntityStatus data structure. |
| [`DCSDoIPEntityStatusGet`](dcsdoipentitystatusget.md) | Specifies the status of a DoIP unit. |
| [`DCSDoIPEntityStatusMaxSockets`](dcsdoipentitystatusmaxsockets.md) | Determines the maximum number of TCP/IP sockets of a DoIP unit from the DCSDoIPEntityStatus data structure. |
| [`DCSDoIPEntityStatusNodeType`](dcsdoipentitystatusnodetype.md) | Determines the type of a DoIP unit from the DCSDoIPEntityStatus data structure. |
| [`DCSDoIPEntityVehicleID`](dcsdoipentityvehicleid.md) | Specifies the vehicle ID of an element from DoIP units in a list. |
| [`DCSDoIPOpen`](dcsdoipopen.md) | Starts a diagnosis session through the IP address without starting the communication with the engine control unit (ECU). |
| [`DCSDoIPRoute`](dcsdoiproute.md) | Specifies the source and destination address of a TCP/IP connection with a DoIP unit. |
| [`DCSDoIPVehicleIDByEntityIDRequest`](dcsdoipvehicleidbyentityidrequest.md) | Sends an UDP request with an entity ID (EID) to all DoIP capable devices in a sub-net so that these devices can identify themselves. |
| [`DCSDoIPVehicleIDByVehicleIDNumberRequest`](dcsdoipvehicleidbyvehicleidnumberrequest.md) | Sends an UDP request with an vehicle ID number (VID) to all DoIP capable devices in a sub-net so that these devices can identify themselves. |
| [`DCSDoIPVehicleIDRequest`](dcsdoipvehicleidrequest.md) | Sends an UDP request to all DoIP capable devices in a sub-net so that these devices can indentify themselves. |
| [`DCSDTCAdditionalDataFromDTCListGet`](dcsdtcadditionaldatafromdtclistget.md) | Determines the optional additional information on a diagnostic trouble code from a list of DTCs. |
| [`DCSDTCClear`](dcsdtcclear.md) | Deletes selected diagnostic trouble codes (DTC). |
| [`DCSDTCCodeFromDTCListGet`](dcsdtccodefromdtclistget.md) | Requests the error code of an element from the DTC list. |
| [`DCSDTCDescriptorInit`](dcsdtcdescriptorinit.md) | Specifies the start of a diagnostic trouble code (DTC). |
| [`DCSDTCGenerationModeSet`](dcsdtcgenerationmodeset.md) | Controls the generation of diagnostic trouble codes (DTC). |
| [`DCSDTCGetByStatus`](dcsdtcgetbystatus.md) | Reads selected diagnostic trouble codes (DTC). |
| [`DCSDTCListSize`](dcsdtclistsize.md) | Specifies the number of diagnostic trouble codes in the list. |
| [`DCSDTCStatusFromDTCListGet`](dcsdtcstatusfromdtclistget.md) | Determines the DTC status of an element from the list. |
| [`DCSDTCStatusGet`](dcsdtcstatusget.md) | Reads selected diagnostic trouble codes. |
| [`DCSECUIDRead`](dcsecuidread.md) | Reads the engine control unit (ECU) ID. |
| [`DCSECUReset`](dcsecureset.md) | Restarts the engine control unit (ECU). |
| [`DCSExtendedCANIDCreate`](dcsextendedcanidcreate.md) | Generates diagnosis-CAN-IDs according to ISO 15765-2. |
| [`DCSIOControl`](dcsiocontrol.md) | Controls the behavior of the I/O port of the engine control unit (ECU). |
| [`DCSISOTPMixedOpen`](dcsisotpmixedopen.md) | Starts a diagnosis session over a CAN port using the ISO TP mixed mode transport protocol. |
| [`DCSISOTPNormalOpen`](dcsisotpnormalopen.md) | Starts a diagnosis session over a CAN port using the ISO TP normal mode transport protocol. |
| [`DCSJ1939AddDataFromDTCListGet`](dcsj1939adddatafromdtclistget.md) | Reads additional data of DTCs from a J1939 Diagnostic Trouble Code (DTCs) list. |
| [`DCSJ1939FMIFromDTCListGet`](dcsj1939fmifromdtclistget.md) | Reads the Failure Mode Identifier (FMI) of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J1939 format. |
| [`DCSJ1939SPNFromDTCListGet`](dcsj1939spnfromdtclistget.md) | Reads the Suspect Parameter Number (SPN) from a Diagnostic Trouble Code (DTC) list which is in J1939 format. |
| [`DCSJ1939StatusFromDTCListGet`](dcsj1939statusfromdtclistget.md) | Reads the status of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J1939 format. |
| [`DCSJ2012AddDataFromDTCListGet`](dcsj2012adddatafromdtclistget.md) | Reads additional data of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J2012 format. |
| [`DCSJ2012DTCFromDTCListGet`](dcsj2012dtcfromdtclistget.md) | Reads the DTC of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J2012 format. |
| [`DCSJ2012FTBFromDTCListGet`](dcsj2012ftbfromdtclistget.md) | Reads a Failure Type Byte (FTB) of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J2012 format. |
| [`DCSJ2012StatusFromDTCListGet`](dcsj2012statusfromdtclistget.md) | Reads the status of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J2012 format. |
| [`DCSLastErrorCodeGet`](dcslasterrorcodeget.md) | Returns the code of the last ADCS error that occurred. |
| [`DCSLastErrorStringGet`](dcslasterrorstringget.md) | Returns the text of the last ADCS error that occurred. |
| [`DCSLINOpen`](dcslinopen.md) | Opens a diagnosis session on an NI-XNET LIN port. |
| [`DCSMemoryRead`](dcsmemoryread.md) | Reads data from the ECU memory. |
| [`DCSMemoryWrite`](dcsmemorywrite.md) | Writes data into the ECU memory. |
| [`DCSNormalMessageTransmissionStart`](dcsnormalmessagetransmissionstart.md) | Starts the standard transmission service. The EDU usually transmits CAN messages. |
| [`DCSNormalMessageTransmissionStop`](dcsnormalmessagetransmissionstop.md) | Ends the standard transmission service. |
| [`DCSOBDCurrentEmissionDTCGet`](dcsobdcurrentemissiondtcget.md) | Reads the emission related diagnostic trouble codes (DTC) of the current test drive cycle. |
| [`DCSOBDEmissionDTCClear`](dcsobdemissiondtcclear.md) | Deletes the emission related diagnostic trouble codes (DTC). |
| [`DCSOBDEmissionDTCGet`](dcsobdemissiondtcget.md) | Deletes the emission related diagnostic trouble codes (DTC). |
| [`DCSOBDOnboardDeviceControlRequest`](dcsobdonboarddevicecontrolrequest.md) | Executes the "Request Control Of On-Board Device". Specifies the behavior of the ECU-I/O ports. |
| [`DCSOBDOpen`](dcsobdopen.md) | Starts a diagnosis session over a CAN port for OBD-II (on-board diagnostic). |
| [`DCSOBDPermanentDTCGet`](dcsobdpermanentdtcget.md) | Reads all permanent diagnostic trouble codes (DTC). |
| [`DCSOBDPowertrainDiagnosticsGet`](dcsobdpowertraindiagnosticsget.md) | Executes an OBD request current powertrain diagnostic data service and reads the data that is acquired. |
| [`DCSOBDPowertrainDTCFreezedDataGet`](dcsobdpowertraindtcfreezeddataget.md) | Executes an OBD request current powertrain freeze frame data service and reads the data that is acquired. |
| [`DCSOBDTestDataRead`](dcsobdtestdataread.md) | Executes an OBD request on-board monitoring test result service and reads the data that is acquired. |
| [`DCSOBDVehicleInformationGet`](dcsobdvehicleinformationget.md) | Reads information from the Engine Control Unit (ECU). |
| [`DCSPropertyGet`](dcspropertyget.md) | Requests a global internal diagnosis parameter. |
| [`DCSPropertySet`](dcspropertyset.md) | Sets a global internal diagnosis property. |
| [`DCSResultGet`](dcsresultget.md) | Requests the results of an ECU routine. |
| [`DCSRoutineStart`](dcsroutinestart.md) | Starts a routine on the engine control unit (ECU). |
| [`DCSRoutineStop`](dcsroutinestop.md) | Stops a routine on the engine control unit (ECU). |
| [`DCSSecurityAccessKeySend`](dcssecurityaccesskeysend.md) | Sends a security check of a key code to the engine control unit (ECU). |
| [`DCSSecurityAccessSeedGet`](dcssecurityaccessseedget.md) | Requests in a security prompt a random number (seed) from the engine control unit (ECU) in order to generate a key code (key). |
| [`DCSTesterPresentServiceExecute`](dcstesterpresentserviceexecute.md) | Executes a Tester Present Service to keep the engine control unit (ECU) in the diagnostic mode. |
| [`DCSTypeDescriptorInit`](dcstypedescriptorinit.md) | Initializes the DCSTypeDescriptor data structure to convert binary data into physical values and vice versa. |
| [`DCSUDS06MemoryRead`](dcsuds06memoryread.md) | Reads data from the memory of the engine control unit (ECU). |
| [`DCSUDS06MemoryWrite`](dcsuds06memorywrite.md) | Writes data into the memory of the engine control unit (ECU). |
| [`DCSUDSCommunicationModeSet`](dcsudscommunicationmodeset.md) | Switches the transmission and the reception of normal messages (mostly CAN messages) on or off. |
| [`DCSUDSDataRead`](dcsudsdataread.md) | Uses a local identifier to read data from the engine control unit (ECU). |
| [`DCSUDSDataWrite`](dcsudsdatawrite.md) | Uses a local identifier to write data onto the engine control unit (ECU). |
| [`DCSUDSDiagnosticModeSet`](dcsudsdiagnosticmodeset.md) | Sets the engine control unit (ECU) into a special diagnosis mode. |
| [`DCSUDSDownloadInit`](dcsudsdownloadinit.md) | Initializes the download of data from the engine control unit (ECU). |
| [`DCSUDSDTCClear`](dcsudsdtcclear.md) | Deletes the selected diagnostic trouble codes (DTC). |
| [`DCSUDSDTCModeSet`](dcsudsdtcmodeset.md) | Switches the generation of diagnostic trouble codes (DTC) on or off. |
| [`DCSUDSECUReset`](dcsudsecureset.md) | Resets the engine control unit (ECU). |
| [`DCSUDSGetDTCBySeverity`](dcsudsgetdtcbyseverity.md) | Executes a weighted status request in order to read selected diagnostic trouble codes (DTC). |
| [`DCSUDSGetDTCByStatus`](dcsudsgetdtcbystatus.md) | Executes a status request in order to read selected diagnostic trouble codes (DTC). |
| [`DCSUDSGetSeverityInformationOfDTC`](dcsudsgetseverityinformationofdtc.md) | Executes a weighted status request in order to read selected diagnostic trouble codes (DTC). |
| [`DCSUDSIOPortModeSet`](dcsudsioportmodeset.md) | Specifies the behavior of the I/O port of the engine control unit (ECU). |
| [`DCSUDSMemoryRead`](dcsudsmemoryread.md) | Reads data from the ECU memory. |
| [`DCSUDSMemoryWrite`](dcsudsmemorywrite.md) | Writes data into the ECU memory. |
| [`DCSUDSRoutineExecute`](dcsudsroutineexecute.md) | Executes a routine on the engine control unit (ECU). |
| [`DCSUDSSecurityAccessKeySend`](dcsudssecurityaccesskeysend.md) | Sends a security check of a key code (key) to the engine control unit (ECU). |
| [`DCSUDSSecurityAccessSeedGet`](dcsudssecurityaccessseedget.md) | Requests in a security prompt a random number (seed) from the engine control unit (ECU) in order to generate a key code (key). |
| [`DCSUDSSupportedDTCGet`](dcsudssupporteddtcget.md) | Reads a list with all supported diagnostic trouble codes (DTCs). |
| [`DCSUDSTesterPresentServiceExecute`](dcsudstesterpresentserviceexecute.md) | Executes a Tester Present Service to keep the engine control unit (ECU) in the diagnostic mode. |
| [`DCSUDSTransmissionTerminate`](dcsudstransmissionterminate.md) | Ends downloading or uploading. |
| [`DCSUDSTransmit`](dcsudstransmit.md) | Transfers data to the engine control unit (ECU) in an upload process or receives data from an ECU in a download process. |
| [`DCSUDSUploadInit`](dcsudsuploadinit.md) | Initiates the data upload onto the engine control unit (ECU). |
| [`DCSVWTPConnect`](dcsvwtpconnect.md) | Creates a connection to the engine control unit (ECU) over the VW TP 2.0 transmission protocol. |
| [`DCSVWTPConnectionTest`](dcsvwtpconnectiontest.md) | Retains a connection to the engine control unit (ECU) over the VW TP 2.0 transmission protocol. |
| [`DCSVWTPDisconnect`](dcsvwtpdisconnect.md) | Disconnects the VW TP 2.0 transmission protocol and the engine control unit (ECU). |
| [`DCSVWTPOpen`](dcsvwtpopen.md) | Starts a diagnosis session over the VW TP 2.0 transmission protocol without starting communication with the engine control unit (ECU). |
| [`DCSWWHConvertDTCsToJ1939`](dcswwhconvertdtcstoj1939.md) | Converts a list with diagnostic trouble codes (DTCs) into the J1939 DTC format. |
| [`DCSWWHConvertDTCsToJ2012`](dcswwhconvertdtcstoj2012.md) | Converts a list with diagnostic trouble codes (DTCs) into the J2012 DTC format. |
| [`DCSWWHDIDRequest`](dcswwhdidrequest.md) | Reads a data set from the ECU. |
| [`DCSWWHDTCExtendedDataRecordRequest`](dcswwhdtcextendeddatarecordrequest.md) | Reads the selected diagnostic trouble codes (DTCs). |
| [`DCSWWHEmissionDTCsClear`](dcswwhemissiondtcsclear.md) | Deletes the selected diagnostic trouble codes (DTCs). |
| [`DCSWWHEmissionDTCsRequest`](dcswwhemissiondtcsrequest.md) | Reads the selected diagnostic trouble codes (DTCs). |
| [`DCSWWHFreezedDataRequest`](dcswwhfreezeddatarequest.md) | Reads the selected diagnostic trouble codes (DTCs). |
| [`DCSWWHRIDRequest`](dcswwhridrequest.md) | Reads a data set from the ECU. |
| [`DCSWWHSupportedDIDsRequest`](dcswwhsupporteddidsrequest.md) | Executes the WWH-OBD ReadDataByIdentifier service in order to get a list of the supported DIDs. |
| [`DCSWWHSupportedRIDsRequest`](dcswwhsupportedridsrequest.md) | Executes the WWH-OBD RoutineControl-Service service in order to get a list of the supported RIDs. |
| [`ECUAxisDataGet`](ecuaxisdataget.md) | Reads the values at the x-axis or y-axis of a characteristic. |
| [`ECUCCPActionService`](ecuccpactionservice.md) | Calls an implementation-specific service on the ECU (CCP only). |
| [`ECUCCPCalibPageGet`](ecuccpcalibpageget.md) | Determines the address of the active data calibration page. |
| [`ECUCCPCalibPageSet`](ecuccpcalibpageset.md) | Specifies that the specified address is the start address for the calibration data page (CCP only). |
| [`ECUCCPDiagnosticService`](ecuccpdiagnosticservice.md) | Calls an implementation-specific diagnostic service on the ECU (CCP only). |
| [`ECUCCPMemoryMove`](ecuccpmemorymove.md) | Moves a memory block on the ECU (CCP only). |
| [`ECUCCPSessionStatusGet`](ecuccpsessionstatusget.md) | Retrieves the current status of the calibration session (CCP only). |
| [`ECUCCPSessionStatusSet`](ecuccpsessionstatusset.md) | Refreshes the ECU with the current status of the calibration session (CCP only). |
| [`ECUCharacteristicGet`](ecucharacteristicget.md) | Reads all data from a specific characteristic on the ECU which is identified by the ECU Reference handle. |
| [`ECUCharacteristicSet`](ecucharacteristicset.md) | Transfers data of a Characteristic to a selected ECU. |
| [`ECUCharacteristicSingleValueGet`](ecucharacteristicsinglevalueget.md) | Reads a single value from a specific Characteristic on the ECU which is identified by the ECU reference handle. |
| [`ECUCharacteristicSingleValueSet`](ecucharacteristicsinglevalueset.md) | Transfers a single value of a Characteristic to a selected ECU. |
| [`ECUChecksumBuild`](ecuchecksumbuild.md) | Calculates a checksum over a defined memory range within the ECU. |
| [`ECUChecksumCreate`](ecuchecksumcreate.md) | Calculates the checksum of a data block in the memory. |
| [`ECUConnect`](ecuconnect.md) | Establishes communication to the selected ECU through CCP or XCP. After a successful ECU connect you can create a measurement task or read/write a characteristic. |
| [`ECUDatabaseClose`](ecudatabaseclose.md) | Closes a specified A2L database. |
| [`ECUDatabaseOpen`](ecudatabaseopen.md) | Opens a specified A2L database. |
| [`ECUDisconnect`](ecudisconnect.md) | Disconnects the CCP communication or XCP communication from the selected ECU. |
| [`ECUDownload`](ecudownload.md) | Downloads data to an ECU. |
| [`ECUMemoryClear`](ecumemoryclear.md) | Clears the contents of the specified ECU memory. |
| [`ECUNameListGet`](ecunamelistget.md) | Calls a list with the names of all ECUs, Measurements, Characteristics, Events, Characteristic pages, or Groups from a specified A2L database. |
| [`ECUProgram`](ecuprogram.md) | Programs a memory block on the ECU. |
| [`ECUProgramReset`](ecuprogramreset.md) | Identifies the end of programming on the ECU. |
| [`ECUProgramStart`](ecuprogramstart.md) | Identifies the start of programming on the ECU. |
| [`ECUPropertyGet`](ecupropertyget.md) | Retrieves the property of the driver, the database, the ECU, the Characteristic, the Measurement, or the Measurement task. |
| [`ECUPropertySet`](ecupropertyset.md) | Sets the property of the driver, the database, the ECU, the Characteristic, the Measurement, or the Measurement task. |
| [`ECUSelect`](ecuselect.md) | Selects an ECU from an A2L database. |
| [`ECUUnselect`](ecuunselect.md) | Deselects an ECU and invalidates the ECU reference handle. |
| [`ECUUpload`](ecuupload.md) | Uploads data from an ECU. |
| [`ECUXCPCalibPageCopy`](ecuxcpcalibpagecopy.md) | Forces a copy operation from one calibration page to another calibration page. |
| [`ECUXCPCalibPageGet`](ecuxcpcalibpageget.md) | Retrieves a setting of the calibration page. |
| [`ECUXCPCalibPageSet`](ecuxcpcalibpageset.md) | Sets a calibration page. |
| [`ECUXCPIdGet`](ecuxcpidget.md) | Retrieves the session configuration or the slave device identification. |
| [`ECUXCPProgramPrepare`](ecuxcpprogramprepare.md) | Prepares the programming of non-volatile memory. |
| [`ECUXCPProgramVerify`](ecuxcpprogramverify.md) | Performs a non-volatile memory certification task on the ECU. |
| [`ECUXCPRequestSet`](ecuxcprequestset.md) | Performs a request to save session and device information to non-volatile memory. |
| [`ECUXCPSegmentModeSet`](ecuxcpsegmentmodeset.md) | Sets the mode of a specified segment. |
| [`ECUXCPStatusGet`](ecuxcpstatusget.md) | Queries the current session status of an ECU slave device. |
| [`MKSCheck`](mkscheck.md) | Checks the definitions and the connections of the loaded block diagram. |
| [`OPCAddGroup`](opcaddgroup.md) | Creates a new OPC group on the OPC server. |
| [`OPCAddItems`](opcadditems.md) | Adds OPC items to an OPC group. |
| [`OPCClear`](opcclear.md) | Disconnects all OPC server connections. |
| [`OPCClearGroup`](opccleargroup.md) | Deletes all OPC items of an OPC group. |
| [`OPCClearItemDef`](opcclearitemdef.md) | Deletes the entries for an OPC item. |
| [`OPCClearServer`](opcclearserver.md) | Deletes all OPC items and OPC groups on an OPC server. |
| [`OPCConnect`](opcconnect.md) | Connects an OPC server. |
| [`OPCDISConnect`](opcdisconnect.md) | Disconnects an OPC server. |
| [`OPCGetAutoValid`](opcgetautovalid.md) | Determines how DIAdem validates OPC items. |
| [`OPCGetBlockParam`](opcgetblockparam.md) | Determines the settings of an OPC block in the block diagram. |
| [`OPCGetConnMode`](opcgetconnmode.md) | Determines the start settings and stop settings for OPC servers. |
| [`OPCGetDouble`](opcgetdouble.md) | Converts a value currently received by the OPC server into a double value and saves the value in the OPCDoubleValue variable. |
| [`OPCGetInt`](opcgetint.md) | Converts a value currently received by the OPC server into a Long value and saves the value in the OPCDoubleValue variable. |
| [`OPCGetLogFile`](opcgetlogfile.md) | Determines whether DIAdem records the OPC communication in a logfile. |
| [`OPCGetSigParam`](opcgetsigparam.md) | Determines the parameters for an OPC signal. |
| [`OPCGetString`](opcgetstring.md) | Converts a value currently received by the OPC server into a string value and saves the value in the OPCStringValue variable. |
| [`OPCLogGetVerb`](opcloggetverb.md) | Determines the settings of the logfile for OPC communication. |
| [`OPCLogSetVerb`](opclogsetverb.md) | Specifies the settings of the logfile for OPC communication. |
| [`OPCReadSync`](opcreadsync.md) | Reads values from items of an OPC group |
| [`OPCRemoveGroup`](opcremovegroup.md) | Deletes OPC groups on OPC servers. |
| [`OPCRemoveItems`](opcremoveitems.md) | Deletes OPC items from an OPC group. |
| [`OPCResetLogFile`](opcresetlogfile.md) | Generates a new logfile for the log of an OPC communication. |
| [`OPCSetActiveFlag`](opcsetactiveflag.md) | Enables or disables the signals in an OPC block. |
| [`OPCSetActiveStat`](opcsetactivestat.md) | Enables or disables OPC items of an OPC group. |
| [`OPCSetArrAccess`](opcsetarraccess.md) | Enables array indexing for the signals of an OPC block. |
| [`OPCSetAutoValid`](opcsetautovalid.md) | Validates OPC items. |
| [`OPCSetCallTo`](opcsetcallto.md) | Restricts the period for unconfirmed OPC operations. |
| [`OPCSetChkAS`](opcsetchkas.md) | Checks asynchronous connections of an OPC block to the OPC server. |
| [`OPCSetConnectTo`](opcsetconnectto.md) | Restricts the period for the link-up to OPC servers. |
| [`OPCSetConnMode`](opcsetconnmode.md) | Specifies when DIAdem starts OPC servers and when DIAdem stops OPC servers. |
| [`OPCSetDeadBand`](opcsetdeadband.md) | Specifies the deadband of an OPC block that works asynchronously. |
| [`OPCSetDeviceRead`](opcsetdeviceread.md) | Specifies how an OPC block reads in data. |
| [`OPCSetDouble`](opcsetdouble.md) | Assigns a Double type value to an OPC server. |
| [`OPCSetErrAction`](opcseterraction.md) | Specifies whether DIAdem cancels the measurement when an OPC block does not receive any values over a certain period of time. |
| [`OPCSetInt`](opcsetint.md) | Assigns a Variant type value to an OPC server. |
| [`OPCSetItemID`](opcsetitemid.md) | Sets the OPC item for a signal and generates the signal name. |
| [`OPCSetLogFile`](opcsetlogfile.md) | Specifies whether DIAdem records the OPC communication in a logfile. |
| [`OPCSetMode`](opcsetmode.md) | Specifies the communication mode for an OPC block. |
| [`OPCSetServer`](opcsetserver.md) | Specifies the OPC server with which an OPC block communicates. |
| [`OPCSetSigName`](opcsetsigname.md) | Specifies a new unique name for an OPC signal. |
| [`OPCSetString`](opcsetstring.md) | Assigns a String type value to an OPC server. |
| [`OPCSetToSync`](opcsettosync.md) | Limits the period of time that an OPC server may wait for the response to asynchronous calls. |
| [`OPCSetUpdRate`](opcsetupdrate.md) | Specifies the time after which the OPC server regularly updates the data in the OPC group. |
| [`OPCSetWaitValid`](opcsetwaitvalid.md) | Specifies whether, and how long, DIAdem waits until the OPC block receives valid measured values from the OPC server. |
| [`OPCSyncListLen`](opcsynclistlen.md) | Adjusts the length of the signal list of an OPC block to the current signal list of the DAC block diagram. |
| [`OPCValidateItems`](opcvalidateitems.md) | Validates the items of an OPC group to add these items to the OPC group. |
| [`OPCWriteSync`](opcwritesync.md) | Writes values to OPC items of an OPC group. |
| [`ScaleMeasDeInit`](scalemeasdeinit.md) | Transfers the results of a calibration measurement to a scaling block. |
| [`ScaleMeasInit`](scalemeasinit.md) | Reads the parameters for a calibration measurement. |
| [`ScaleMeasVal1Get`](scalemeasval1get.md) | Determines the first value of the input range of a calibration measurement. |
| [`ScaleMeasVal2Get`](scalemeasval2get.md) | Determines the second value of the input range of a calibration measurement. |
| [`SchemeCheck`](schemecheck.md) | Transfers a block diagram into the measurement kernel and checks this block diagram. |
| [`SchemeDel`](schemedel.md) | Deletes all DAC blocks and all buses in the open block diagram or sub-block diagram. |
| [`SchemeExp`](schemeexp.md) | Saves the currently open subblock diagram. |
| [`SchemeImp`](schemeimp.md) | Imports the specified subblock diagram file in the new subblock diagram of the existing block diagram. |
| [`SchemeLoad`](schemeload.md) | Loads a block diagram. |
| [`SchemeMeasOnly`](schememeasonly.md) | Starts a measurement with data storage without visualizing the data in DIAdem VISUAL. A measurement without visualization can attain high sampling rates. |
| [`SchemeMeasStart`](schememeasstart.md) | Starts a measurement with data storage and visualizes the data in DIAdem VISUAL. |
| [`SchemeMeasTest`](schememeastest.md) | Starts a measurement without data storage and visualizes the data in DIAdem VISUAL. |
| [`SchemeNew`](schemenew.md) | Deletes the entire DAC block diagram. |
| [`SchemePrint`](schemeprint.md) | Prints out the loaded block diagram or the open subblock diagram. |
| [`SchemeSave`](schemesave.md) | Saves the current block diagram under a new name. |
| [`SchemeUpdate`](schemeupdate.md) | Refreshes the display of a block diagram in DIAdem DAC. |
| [`VisUpdate`](visupdate.md) | Refreshes the displays in DIAdem VISUAL. |
