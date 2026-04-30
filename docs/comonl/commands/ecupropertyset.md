---
title: "ECUPropertySet"
description: "Sets the property of the driver, the database, the ECU, the Characteristic, the Measurement, or the Measurement task."
---

# ECUPropertySet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUPropertySet

Sets the property of the driver, the database, the ECU, the Characteristic, the Measurement, or the Measurement task.

## Signature

```python
dd.ECUPropertySet(ECUHandle, ECUName, ECUPropertyID, ECUPropertyValue)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ECUHandle</td>
<td>Specifies the handle you use to access the ECU.<div id="exp_ECUHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a>F</td></tr>
<tr>
<td>-21474836487 &lt;= ECUHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUName</td>
<td>Specifies the name for accessing an element in an A2L database file. This name is, for example, the name of an ECU, a Characteristic, or a Measurement.<div id="exp_ECUName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUPropertyID</td>
<td>Specifies the property.<div id="exp_ECUPropertyID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUPropertyID &lt;= 2147483647</td></tr>
</table>
<p class="Body">The variable can accept the following values:</p>
<table class="Borderless">
<tr><td>0</td><td width="150"><span class="Monospace">eECUPropertyGenVersionMajor</span></td><td>Contains the main version number of the ECU measurement and calibration toolkit.</td></tr>
<tr><td>1</td><td width="150"><span class="Monospace">eECUPropertyGenVersionMinor</span></td><td>Contains the sub-version number of the ECU measurement and calibration toolkit.</td></tr>
<tr><td>2</td><td width="150"><span class="Monospace">eECUPropertyGenVersionUpdate</span></td><td>Contains the update version number of the ECU measurement and calibration toolkit.</td></tr>
<tr><td>3</td><td width="150"><span class="Monospace">eECUPropertyGenVersionBuild</span></td><td>Contains the build number of the ECU measurement and calibration toolkit.</td></tr>
<tr><td>4</td><td width="150"><span class="Monospace">eECUPropertyGenVersionComment</span></td><td>Contains a comment from the ECU measurement and calibration toolkit.</td></tr>
<tr><td>256</td><td width="150"><span class="Monospace">eECUPropertyDBFilename</span></td><td>Contains the filename of the A2L database which opened the task.</td></tr>
<tr><td>512</td><td width="150"><span class="Monospace">eECUPropertyECUDTOID</span></td><td>Contains the DTO-ID (Data Transmission Object), which the ECU uses to react to CCP commands and to send data and status information to the CCP master.</td></tr>
<tr><td>513</td><td width="150"><span class="Monospace">eECUPropertyECUCROID</span></td><td>Contains the CRO-ID (Command Receive Object), which the ECU uses to send commands and data from the host to the slave device.</td></tr>
<tr><td>515</td><td width="150"><span class="Monospace">eECUPropertyECUInterface</span></td><td>Contains the interface initialized for the task.</td></tr>
<tr><td>516</td><td width="150"><span class="Monospace">eECUPropertyECUBaudRate</span></td><td>Contains the transfer rate.</td></tr>
<tr><td>517</td><td width="150"><span class="Monospace">eECUPropertyECUStationAddress</span></td><td>Contains the station address of the slave device. CCP can use several control devices with the same CAN arbitration ID for the CCP communication. To avoid communication conflicts, CCP specifies a unique station address for all control devices.</td></tr>
<tr><td>518</td><td width="150"><span class="Monospace">eECUPropertyECUByteOrder</span></td><td>Contains the byte order of the slave device. 0 or MSB_LAST specify the Intel format which sorts the bytes in the Little-Endian order with the lowest bit first. 1 or MSB_FIRST specify the Motorola format which sorts the bytes in the Little-Endian order with the highest bit first.</td></tr>
<tr><td>519</td><td width="150"><span class="Monospace">eECUPropertyECUSeedKeyCal</span></td><td>Contains the filename of the SeedKey-DLL used for the calibration.</td></tr>
<tr><td>520</td><td width="150"><span class="Monospace">eECUPropertyECUSeedKeyDAQ</span></td><td>Contains the filename of the SeedKey-DLL used for DAQ.</td></tr>
<tr><td>521</td><td width="150"><span class="Monospace">eECUPropertyECUSeedKeyProg</span></td><td>Contains the filename of the SeedKey-DLL used for the programming.</td></tr>
<tr><td>522</td><td width="150"><span class="Monospace">eECUPropertyECUChecksum</span></td><td>Contains the filename of the DLL used for checking the checksum.</td></tr>
<tr><td>523</td><td width="150"><span class="Monospace">eECUPropertyECUName</span></td><td>Contains the name of the selected ECU.</td></tr>
<tr><td>524</td><td width="150"><span class="Monospace">eECUPropertyECUMasterID</span></td><td>Contains the CCP master ID. This property is optional and depends on the ECU implementation.</td></tr>
<tr><td>525</td><td width="150"><span class="Monospace">eECUPropertyECUIDDataType</span></td><td>Contains the data type of the slave device ID. This property is optional and depends on the ECU implementation.</td></tr>
<tr><td>526</td><td width="150"><span class="Monospace">eECUPropertyECUIDLength</span></td><td>Contains the size of the slave device ID in bytes.</td></tr>
<tr><td>527</td><td width="150"><span class="Monospace">eECUPropertyECUID</span></td><td>Contains the slave device ID. This property is optional and depends on the ECU implementation.</td></tr>
<tr><td>535</td><td width="150"><span class="Monospace">eECUPropertyECUSingleByteDAQLists</span></td><td>Contains whether an ECU supports single byte or multi-byte DAQ list entries.</td></tr>
<tr><td>536</td><td width="150"><span class="Monospace">eECUPropertyECUTimingFactor</span></td><td>Contains a value for increasing the timeout values of CCP or XCP commands through multiplication.</td></tr>
<tr><td>544</td><td width="150"><span class="Monospace">eECUPropertyECUCmdByteOrder</span></td><td>Contains the byte order of the multi-byte command parameters. 0 or MSB_LAST specify the Intel format for the slave device which sorts the bytes in the Little-Endian order with the lowest bit first. 1 or MSB_LAST specify the Motorola format for the slave device which sorts the bytes in the Big-Endian order with the highest bit first.</td></tr>
<tr><td>545</td><td width="150"><span class="Monospace">eECUPropertyECUSeedKeyXCP</span></td><td>Contains the filename of the SeedKey-DLL used for XCP.</td></tr>
<tr><td>548</td><td width="150"><span class="Monospace">eECUPropertyECUDAQListNumbers</span></td><td>Contains the numbers of all DAQ lists contained in the A2L file.</td></tr>
<tr><td>558</td><td width="150"><span class="Monospace">eECUPropertyECUSeedChkDllPath</span></td><td>Contains the folder and its path in which the ECU Measurement and Calibration toolkit searches for the SeedKey or checksum DLL. If the property specifies an empty string, the ECU Measurement and Calibration toolkit expects the DLLs in the same folder that the A2L file specifies.</td></tr>
<tr><td>768</td><td width="150"><span class="Monospace">eECUPropertyMeasAddress</span></td><td>Contains the address of the selected measurement in the control device memory.</td></tr>
<tr><td>769</td><td width="150"><span class="Monospace">eECUPropertyMeasExtension</span></td><td>Contains additional address information about the ECU address in the A2L database.</td></tr>
<tr><td>770</td><td width="150"><span class="Monospace">eECUPropertyMeasDatatype</span></td><td>Contains the data type of the measurement task.</td></tr>
<tr><td>771</td><td width="150"><span class="Monospace">eECUPropertyMeasByteOrder</span></td><td>Contains the byte order. 0 specifies the Intel format which sorts the bytes in the Little-Endian order with the lowest bit first. 1 specifies the Motorola format which sorts the bytes in the Little-Endian order with the highest bit first.</td></tr>
<tr><td>772</td><td width="150"><span class="Monospace">eECUPropertyMeasMaximum</span></td><td>Contains the maximum value of the measurement.</td></tr>
<tr><td>773</td><td width="150"><span class="Monospace">eECUPropertyMeasMinimum</span></td><td>Contains the minimum value of the measurement.</td></tr>
<tr><td>774</td><td width="150"><span class="Monospace">eECUPropertyMeasReadOnly</span></td><td>Contains whether the measurement is read only.</td></tr>
<tr><td>775</td><td width="150"><span class="Monospace">eECUPropertyMeasIsVirtual</span></td><td>Contains whether the measurement is virtual. ECU does not transfer virtual measurements. They are calculated in the application.</td></tr>
<tr><td>777</td><td width="150"><span class="Monospace">eECUPropertyMeasUnit</span></td><td>Contains the unit of the measurement.</td></tr>
<tr><td>779</td><td width="150"><span class="Monospace">eECUPropertyMeasComment</span></td><td>Contains a comment.</td></tr>
<tr><td>780</td><td width="150"><span class="Monospace">eECUPropertyMeasScaleFactor</span></td><td>Contains the scaling factor of the measurement.</td></tr>
<tr><td>781</td><td width="150"><span class="Monospace">eECUPropertyMeasScaleOffset</span></td><td>Contains the scaling offset of the measurement.</td></tr>
<tr><td>782</td><td width="150"><span class="Monospace">eECUPropertyMeasScaleType</span></td><td>Contains the scaling type of the measurement.</td></tr>
<tr><td>1024</td><td width="150"><span class="Monospace">eECUPropertyCharAddress</span></td><td>Contains the address of the selected characteristic in the ECU memory.</td></tr>
<tr><td>1025</td><td width="150"><span class="Monospace">eECUPropertyCharExtension</span></td><td>Contains additional address information, for example, to distinguish different address areas in an ECU.</td></tr>
<tr><td>1026</td><td width="150"><span class="Monospace">eECUPropertyCharDatatype</span></td><td>Contains the data type of the characteristic.</td></tr>
<tr><td>1027</td><td width="150"><span class="Monospace">eECUPropertyCharByteOrder</span></td><td>Contains the byte order. 0 specifies the Intel format which sorts the bytes in the Little-Endian order with the lowest bit first. 1 specifies the Motorola format which sorts the bytes in the Little-Endian order with the highest bit first.</td></tr>
<tr><td>1028</td><td width="150"><span class="Monospace">eECUPropertyCharDimension</span></td><td>Contains the dimension of the characteristic.</td></tr>
<tr><td>1029</td><td width="150"><span class="Monospace">eECUPropertyCharSizes</span></td><td>Contains the size of the characteristic.</td></tr>
<tr><td>1030</td><td width="150"><span class="Monospace">eECUPropertyCharXAxis</span></td><td>Contains the characteristic defined for the x-axis values.</td></tr>
<tr><td>1031</td><td width="150"><span class="Monospace">eECUPropertyCharYAxis</span></td><td>Contains the characteristic defined for the y-axis values.</td></tr>
<tr><td>1032</td><td width="150"><span class="Monospace">eECUPropertyCharMaximum</span></td><td>Contains the maximum value of the characteristic.</td></tr>
<tr><td>1033</td><td width="150"><span class="Monospace">eECUPropertyCharMinimum</span></td><td>Contains the minimum value of the characteristic.</td></tr>
<tr><td>1034</td><td width="150"><span class="Monospace">eECUPropertyCharReadOnly</span></td><td>Contains whether the characteristic is read only.</td></tr>
<tr><td>1036</td><td width="150"><span class="Monospace">eECUPropertyCharUnit</span></td><td>Contains the unit of the characteristic.</td></tr>
<tr><td>1038</td><td width="150"><span class="Monospace">eECUPropertyCharComment</span></td><td>Contains the comment from the ECU measurement and calibration toolkit.</td></tr>
<tr><td>1039</td><td width="150"><span class="Monospace">eECUPropertyCharScaleFactor</span></td><td>Contains the scaling factor of the characteristic.</td></tr>
<tr><td>1040</td><td width="150"><span class="Monospace">eECUPropertyCharScaleOffset</span></td><td>Contains the scaling offset of the characteristic.</td></tr>
<tr><td>1041</td><td width="150"><span class="Monospace">eECUPropertyCharScaleType</span></td><td>Contains the scaling type of the characteristic.</td></tr>
<tr><td>0</td><td width="150"><span class="Monospace">eECUPropertyGroupIsRoot</span></td><td>Contains the information whether a specific group is a root group, which is a group without parents.</td></tr>
<tr><td>1280</td><td width="150"><span class="Monospace">eECUPropertyDAQMode</span></td><td>Contains the selected mode of an M&amp;C measurement task. 0-DAQ list specifies that the data defined in the A2L data base is transferred from ECU in equidistant time intervals. 1 polling specifies that the data are loaded by the ECU after the ECUDAQRead from the measurement task is called.</td></tr>
<tr><td>1291</td><td width="150"><span class="Monospace">eECUPropertyDAQListCANId</span></td><td>Contains the CAN ID.</td></tr>
<tr><td>1292</td><td width="150"><span class="Monospace">eECUPropertyDAQListFirstPID</span></td><td>Contains the first packet ID of the specified DAQ list.</td></tr>
<tr><td>1293</td><td width="150"><span class="Monospace">eECUPropertyDAQListNumberOfEventChannels</span></td><td>Contains the number of permitted event channels of the specified DAQ list.</td></tr>
<tr><td>1294</td><td width="150"><span class="Monospace">eECUPropertyDAQListEventChannels</span></td><td>Contains the number of permitted event channels for the specified DAQ list.</td></tr>
<tr><td>1295</td><td width="150"><span class="Monospace">eECUPropertyDAQListReductionAllowed</span></td><td>Contains whether the specified DAQ list supports a reduction of the transfer rate.</td></tr>
<tr><td>1296</td><td width="150"><span class="Monospace">eECUPropertyDAQListNumberOfExcludedDAQLists</span></td><td>Contains the size of the field with the DAQ list numbers which do not function with the current DAQ list.</td></tr>
<tr><td>1297</td><td width="150"><span class="Monospace">eECUPropertyDAQListExcludedDAQLists</span></td><td>Contains the DAQ list numbers which do not function with the current DAQ list.</td></tr>
<tr><td>0</td><td width="150"><span class="Monospace">eECUPropertyIPAddress</span></td><td>Contains the IP address for XCP in Ethernet (TCP or UDP) as a string.</td></tr>
<tr><td>2</td><td width="150"><span class="Monospace">eECUPropertyIPPort</span></td><td>Contains the IP port for XCP in Ethernet (TCP or UDP).</td></tr>
<tr><td>16</td><td width="150"><span class="Monospace">eECUPropertyDTOID</span></td><td>Contains which DTO-ID (Data Transmission Object) is used to send data from the DAQ lists to the CCP master.</td></tr>
<tr><td>17</td><td width="150"><span class="Monospace">eECUPropertyCROID</span></td><td>Contains the CRO-ID (Command Receive Object) used to send commands and data from the host to the slave device.</td></tr>
<tr><td>18</td><td width="150"><span class="Monospace">eECUPropertyCANBaudrate</span></td><td>Contains the CAN baud rate for CCP or XCP which are used for sending commands and data from the host to the slave device.</td></tr>
<tr><td>1792</td><td width="150"><span class="Monospace">eECUPropertyPGMCompressionMethod</span></td><td>Contains the selected compression method for the ECU program.</td></tr>
<tr><td>1793</td><td width="150"><span class="Monospace">eECUPropertyPGMEncryptionMethod</span></td><td>Contains the selected encrypting method for ECUProgram.</td></tr>
<tr><td>1794</td><td width="150"><span class="Monospace">eECUPropertyPGMProgrammingMethod</span></td><td>Contains the selected programming method for ECUProgram.</td></tr>
<tr><td>1795</td><td width="150"><span class="Monospace">eECUPropertyPGMAccessMethod</span></td><td>Contains the selected accessing method for ECUProgram and ECUMemoryClear.</td></tr>
<tr><td>2048</td><td width="150"><span class="Monospace">eECUPropertyCRCBitReflection</span></td><td>Specifies whether the CRC checksum is calculated with reversed bits.</td></tr>
<tr><td>2049</td><td width="150"><span class="Monospace">eECUPropertyCRCStartValue</span></td><td>Specifies the start value for the checksum.</td></tr>
<tr><td>2304</td><td width="150"><span class="Monospace">eECUPropertyOptCmdGETSEED</span></td><td>Contains whether the ECU supports the optional CCP command GET_SEED.</td></tr>
<tr><td>2305</td><td width="150"><span class="Monospace">eECUPropertyOptCmdUNLOCK</span></td><td>Contains whether the ECU supports the optional CCP command UNLOCK.</td></tr>
<tr><td>2306</td><td width="150"><span class="Monospace">eECUPropertyOptCmdDNLOAD6</span></td><td>Contains whether the ECU supports the optional CCP command DNLOAD_6.</td></tr>
<tr><td>2307</td><td width="150"><span class="Monospace">eECUPropertyOptCmdSHORTUP</span></td><td>Contains whether the ECU supports the optional CCP command  SHORT_UP.</td></tr>
<tr><td>2308</td><td width="150"><span class="Monospace">eECUPropertyOptCmdSELECTCALPAGE</span></td><td>Contains whether the ECU supports the optional CCP command  SELECT_CAL_PAGE.</td></tr>
<tr><td>2309</td><td width="150"><span class="Monospace">eECUPropertyOptCmdSETSSTATUS</span></td><td>Contains whether the ECU supports the optional CCP command SET_S_STATUS.</td></tr>
<tr><td>2310</td><td width="150"><span class="Monospace">eECUPropertyOptCmdGETSSTATUS</span></td><td>Contains whether the ECU supports the optional CCP command GET_S_STATUS.</td></tr>
<tr><td>2311</td><td width="150"><span class="Monospace">eECUPropertyOptCmdBUILDCHKSUM</span></td><td>Contains whether the ECU supports the optional CCP command BUILD_CHKSUM.</td></tr>
<tr><td>2312</td><td width="150"><span class="Monospace">eECUPropertyOptCmdCLEARMEMORY</span></td><td>Contains whether the ECU supports the optional CCP command CLEAR_MEMORY.</td></tr>
<tr><td>2313</td><td width="150"><span class="Monospace">eECUPropertyOptCmdPROGRAM</span></td><td>Contains whether the ECU supports the optional CCP command PROGRAM.</td></tr>
<tr><td>2314</td><td width="150"><span class="Monospace">eECUPropertyOptCmdPROGRAM6</span></td><td>Contains whether the ECU supports the optional CCP command PROGRAM_6.</td></tr>
<tr><td>2315</td><td width="150"><span class="Monospace">eECUPropertyOptCmdMOVE</span></td><td>Contains whether the ECU supports the optional CCP command MOVE.</td></tr>
<tr><td>2316</td><td width="150"><span class="Monospace">eECUPropertyOptCmdTEST</span></td><td>Contains whether the ECU supports the optional CCP command TEST.</td></tr>
<tr><td>2317</td><td width="150"><span class="Monospace">eECUPropertyOptCmdGETACTIVECALPAGE</span></td><td>Contains whether the ECU supports the optional CCP command GET_ACTIVE_CAL_PAGE.</td></tr>
<tr><td>2318</td><td width="150"><span class="Monospace">eECUPropertyOptCmdSTARTSTOPALL</span></td><td>Contains whether the ECU supports the optional CCP command START_STOP_ALL.</td></tr>
<tr><td>2319</td><td width="150"><span class="Monospace">eECUPropertyOptCmdDIAGSERVICE</span></td><td>Contains whether the ECU supports the optional CCP command DIAG_SERVICE.</td></tr>
<tr><td>2320</td><td width="150"><span class="Monospace">eECUPropertyOptCmdACTIONSERVICE</span></td><td>Contains whether the ECU supports the optional CCP command ACTION_SERVICE.</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUPropertyValue</td>
<td>Specifies the value of the property.<div id="exp_ECUPropertyValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eECUPropertyGenVersionMajor` | 0 | Contains the main version number of the ECU measurement and calibration toolkit. |
| `eECUPropertyGenVersionMinor` | 1 | Contains the sub-version number of the ECU measurement and calibration toolkit. |
| `eECUPropertyGenVersionUpdate` | 2 | Contains the update version number of the ECU measurement and calibration toolkit. |
| `eECUPropertyGenVersionBuild` | 3 | Contains the build number of the ECU measurement and calibration toolkit. |
| `eECUPropertyGenVersionComment` | 4 | Contains a comment from the ECU measurement and calibration toolkit. |
| `eECUPropertyDBFilename` | 256 | Contains the filename of the A2L database which opened the task. |
| `eECUPropertyECUDTOID` | 512 | Contains the DTO-ID (Data Transmission Object), which the ECU uses to react to CCP commands and to send data and status information to the CCP master. |
| `eECUPropertyECUCROID` | 513 | Contains the CRO-ID (Command Receive Object), which the ECU uses to send commands and data from the host to the slave device. |
| `eECUPropertyECUInterface` | 515 | Contains the interface initialized for the task. |
| `eECUPropertyECUBaudRate` | 516 | Contains the transfer rate. |
| `eECUPropertyECUStationAddress` | 517 | Contains the station address of the slave device. CCP can use several control devices with the same CAN arbitration ID for the CCP communication. To avoid communication conflicts, CCP specifies a unique station address for all control devices. |
| `eECUPropertyECUByteOrder` | 518 | Contains the byte order of the slave device. 0 or MSB_LAST specify the Intel format which sorts the bytes in the Little-Endian order with the lowest bit first. 1 or MSB_FIRST specify the Motorola format which sorts the bytes in the Little-Endian order with the highest bit first. |
| `eECUPropertyECUSeedKeyCal` | 519 | Contains the filename of the SeedKey-DLL used for the calibration. |
| `eECUPropertyECUSeedKeyDAQ` | 520 | Contains the filename of the SeedKey-DLL used for DAQ. |
| `eECUPropertyECUSeedKeyProg` | 521 | Contains the filename of the SeedKey-DLL used for the programming. |
| `eECUPropertyECUChecksum` | 522 | Contains the filename of the DLL used for checking the checksum. |
| `eECUPropertyECUName` | 523 | Contains the name of the selected ECU. |
| `eECUPropertyECUMasterID` | 524 | Contains the CCP master ID. This property is optional and depends on the ECU implementation. |
| `eECUPropertyECUIDDataType` | 525 | Contains the data type of the slave device ID. This property is optional and depends on the ECU implementation. |
| `eECUPropertyECUIDLength` | 526 | Contains the size of the slave device ID in bytes. |
| `eECUPropertyECUID` | 527 | Contains the slave device ID. This property is optional and depends on the ECU implementation. |
| `eECUPropertyECUSingleByteDAQLists` | 535 | Contains whether an ECU supports single byte or multi-byte DAQ list entries. |
| `eECUPropertyECUTimingFactor` | 536 | Contains a value for increasing the timeout values of CCP or XCP commands through multiplication. |
| `eECUPropertyECUCmdByteOrder` | 544 | Contains the byte order of the multi-byte command parameters. 0 or MSB_LAST specify the Intel format for the slave device which sorts the bytes in the Little-Endian order with the lowest bit first. 1 or MSB_LAST specify the Motorola format for the slave device which sorts the bytes in the Big-Endian order with the highest bit first. |
| `eECUPropertyECUSeedKeyXCP` | 545 | Contains the filename of the SeedKey-DLL used for XCP. |
| `eECUPropertyECUDAQListNumbers` | 548 | Contains the numbers of all DAQ lists contained in the A2L file. |
| `eECUPropertyECUSeedChkDllPath` | 558 | Contains the folder and its path in which the ECU Measurement and Calibration toolkit searches for the SeedKey or checksum DLL. If the property specifies an empty string, the ECU Measurement and Calibration toolkit expects the DLLs in the same folder that the A2L file specifies. |
| `eECUPropertyMeasAddress` | 768 | Contains the address of the selected measurement in the control device memory. |
| `eECUPropertyMeasExtension` | 769 | Contains additional address information about the ECU address in the A2L database. |
| `eECUPropertyMeasDatatype` | 770 | Contains the data type of the measurement task. |
| `eECUPropertyMeasByteOrder` | 771 | Contains the byte order. 0 specifies the Intel format which sorts the bytes in the Little-Endian order with the lowest bit first. 1 specifies the Motorola format which sorts the bytes in the Little-Endian order with the highest bit first. |
| `eECUPropertyMeasMaximum` | 772 | Contains the maximum value of the measurement. |
| `eECUPropertyMeasMinimum` | 773 | Contains the minimum value of the measurement. |
| `eECUPropertyMeasReadOnly` | 774 | Contains whether the measurement is read only. |
| `eECUPropertyMeasIsVirtual` | 775 | Contains whether the measurement is virtual. ECU does not transfer virtual measurements. They are calculated in the application. |
| `eECUPropertyMeasUnit` | 777 | Contains the unit of the measurement. |
| `eECUPropertyMeasComment` | 779 | Contains a comment. |
| `eECUPropertyMeasScaleFactor` | 780 | Contains the scaling factor of the measurement. |
| `eECUPropertyMeasScaleOffset` | 781 | Contains the scaling offset of the measurement. |
| `eECUPropertyMeasScaleType` | 782 | Contains the scaling type of the measurement. |
| `eECUPropertyCharAddress` | 1024 | Contains the address of the selected characteristic in the ECU memory. |
| `eECUPropertyCharExtension` | 1025 | Contains additional address information, for example, to distinguish different address areas in an ECU. |
| `eECUPropertyCharDatatype` | 1026 | Contains the data type of the characteristic. |
| `eECUPropertyCharByteOrder` | 1027 | Contains the byte order. 0 specifies the Intel format which sorts the bytes in the Little-Endian order with the lowest bit first. 1 specifies the Motorola format which sorts the bytes in the Little-Endian order with the highest bit first. |
| `eECUPropertyCharDimension` | 1028 | Contains the dimension of the characteristic. |
| `eECUPropertyCharSizes` | 1029 | Contains the size of the characteristic. |
| `eECUPropertyCharXAxis` | 1030 | Contains the characteristic defined for the x-axis values. |
| `eECUPropertyCharYAxis` | 1031 | Contains the characteristic defined for the y-axis values. |
| `eECUPropertyCharMaximum` | 1032 | Contains the maximum value of the characteristic. |
| `eECUPropertyCharMinimum` | 1033 | Contains the minimum value of the characteristic. |
| `eECUPropertyCharReadOnly` | 1034 | Contains whether the characteristic is read only. |
| `eECUPropertyCharUnit` | 1036 | Contains the unit of the characteristic. |
| `eECUPropertyCharComment` | 1038 | Contains the comment from the ECU measurement and calibration toolkit. |
| `eECUPropertyCharScaleFactor` | 1039 | Contains the scaling factor of the characteristic. |
| `eECUPropertyCharScaleOffset` | 1040 | Contains the scaling offset of the characteristic. |
| `eECUPropertyCharScaleType` | 1041 | Contains the scaling type of the characteristic. |
| `eECUPropertyGroupIsRoot` | 0 | Contains the information whether a specific group is a root group, which is a group without parents. |
| `eECUPropertyDAQMode` | 1280 | Contains the selected mode of an M&C measurement task. 0-DAQ list specifies that the data defined in the A2L data base is transferred from ECU in equidistant time intervals. 1 polling specifies that the data are loaded by the ECU after the ECUDAQRead from the measurement task is called. |
| `eECUPropertyDAQListCANId` | 1291 | Contains the CAN ID. |
| `eECUPropertyDAQListFirstPID` | 1292 | Contains the first packet ID of the specified DAQ list. |
| `eECUPropertyDAQListNumberOfEventChannels` | 1293 | Contains the number of permitted event channels of the specified DAQ list. |
| `eECUPropertyDAQListEventChannels` | 1294 | Contains the number of permitted event channels for the specified DAQ list. |
| `eECUPropertyDAQListReductionAllowed` | 1295 | Contains whether the specified DAQ list supports a reduction of the transfer rate. |
| `eECUPropertyDAQListNumberOfExcludedDAQLists` | 1296 | Contains the size of the field with the DAQ list numbers which do not function with the current DAQ list. |
| `eECUPropertyDAQListExcludedDAQLists` | 1297 | Contains the DAQ list numbers which do not function with the current DAQ list. |
| `eECUPropertyIPAddress` | 0 | Contains the IP address for XCP in Ethernet (TCP or UDP) as a string. |
| `eECUPropertyIPPort` | 2 | Contains the IP port for XCP in Ethernet (TCP or UDP). |
| `eECUPropertyDTOID` | 16 | Contains which DTO-ID (Data Transmission Object) is used to send data from the DAQ lists to the CCP master. |
| `eECUPropertyCROID` | 17 | Contains the CRO-ID (Command Receive Object) used to send commands and data from the host to the slave device. |
| `eECUPropertyCANBaudrate` | 18 | Contains the CAN baud rate for CCP or XCP which are used for sending commands and data from the host to the slave device. |
| `eECUPropertyPGMCompressionMethod` | 1792 | Contains the selected compression method for the ECU program. |
| `eECUPropertyPGMEncryptionMethod` | 1793 | Contains the selected encrypting method for ECUProgram. |
| `eECUPropertyPGMProgrammingMethod` | 1794 | Contains the selected programming method for ECUProgram. |
| `eECUPropertyPGMAccessMethod` | 1795 | Contains the selected accessing method for ECUProgram and ECUMemoryClear. |
| `eECUPropertyCRCBitReflection` | 2048 | Specifies whether the CRC checksum is calculated with reversed bits. |
| `eECUPropertyCRCStartValue` | 2049 | Specifies the start value for the checksum. |
| `eECUPropertyOptCmdGETSEED` | 2304 | Contains whether the ECU supports the optional CCP command GET_SEED. |
| `eECUPropertyOptCmdUNLOCK` | 2305 | Contains whether the ECU supports the optional CCP command UNLOCK. |
| `eECUPropertyOptCmdDNLOAD6` | 2306 | Contains whether the ECU supports the optional CCP command DNLOAD_6. |
| `eECUPropertyOptCmdSHORTUP` | 2307 | Contains whether the ECU supports the optional CCP command  SHORT_UP. |
| `eECUPropertyOptCmdSELECTCALPAGE` | 2308 | Contains whether the ECU supports the optional CCP command  SELECT_CAL_PAGE. |
| `eECUPropertyOptCmdSETSSTATUS` | 2309 | Contains whether the ECU supports the optional CCP command SET_S_STATUS. |
| `eECUPropertyOptCmdGETSSTATUS` | 2310 | Contains whether the ECU supports the optional CCP command GET_S_STATUS. |
| `eECUPropertyOptCmdBUILDCHKSUM` | 2311 | Contains whether the ECU supports the optional CCP command BUILD_CHKSUM. |
| `eECUPropertyOptCmdCLEARMEMORY` | 2312 | Contains whether the ECU supports the optional CCP command CLEAR_MEMORY. |
| `eECUPropertyOptCmdPROGRAM` | 2313 | Contains whether the ECU supports the optional CCP command PROGRAM. |
| `eECUPropertyOptCmdPROGRAM6` | 2314 | Contains whether the ECU supports the optional CCP command PROGRAM_6. |
| `eECUPropertyOptCmdMOVE` | 2315 | Contains whether the ECU supports the optional CCP command MOVE. |
| `eECUPropertyOptCmdTEST` | 2316 | Contains whether the ECU supports the optional CCP command TEST. |
| `eECUPropertyOptCmdGETACTIVECALPAGE` | 2317 | Contains whether the ECU supports the optional CCP command GET_ACTIVE_CAL_PAGE. |
| `eECUPropertyOptCmdSTARTSTOPALL` | 2318 | Contains whether the ECU supports the optional CCP command START_STOP_ALL. |
| `eECUPropertyOptCmdDIAGSERVICE` | 2319 | Contains whether the ECU supports the optional CCP command DIAG_SERVICE. |
| `eECUPropertyOptCmdACTIONSERVICE` | 2320 | Contains whether the ECU supports the optional CCP command ACTION_SERVICE. |

---

*Source: `ComOnl/ECUPropertySet.htm`*
