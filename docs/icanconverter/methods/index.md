---
title: "Methods (ICANConverter)"
---

# Methods

47 methods from `ICANConverter.chm`.

| Name | Summary |
| --- | --- |
| [`IBusCollection.Add`](ibuscollection-add.md) | Use the AddByType instead of the Add method in order to add a bus to the Buses collection and to specify the bus type. Adds a bus to the Buses collection in the Bus Log Converter . |
| [`IBusCollection.AddByType`](ibuscollection-addbytype.md) | Adds a bus of a specific type to the Buses collection in the Bus Log Converter . |
| [`IBusCollection.Exists`](ibuscollection-exists.md) | Checks whether a bus with a specific name already exists in the Bus Log Converter . |
| [`IBusCollection.ExistsBusNo`](ibuscollection-existsbusno.md) | Use the ExistsBusNoByType method instead of the ExistsBusNo method to check whether a bus with a certain number and a specific type already exists in the Buses collection. Checks in the Bus Log Converter whether a CAN bus with a specific number already exists. |
| [`IBusCollection.ExistsBusNoByType`](ibuscollection-existsbusnobytype.md) | Checks in the Bus Log Converter whether a bus with a certain number and a specific type already exists in the Buses collection. |
| [`IBusCollection.GetIndex`](ibuscollection-getindex.md) | Returns the index of a bus from the Buses collection in the Bus Log Converter . |
| [`IBusCollection.Item`](ibuscollection-item.md) | Returns the bus that is associated with a specific index or name in the Bus Log Converter . |
| [`IBusCollection.Move`](ibuscollection-move.md) | Moves a bus in the Buses collection to the specified position, in the Bus Log Converter . |
| [`IBusCollection.Remove`](ibuscollection-remove.md) | Deletes an element from the Buses collection , in the Bus Log Converter . |
| [`IBusCollection.RemoveAll`](ibuscollection-removeall.md) | Deletes all elements from the Buses collection , in the Bus Log Converter . |
| [`IBusFilterBusCollection.Add`](ibusfilterbuscollection-add.md) | Adds a bus to the UsedBuses collection in the Bus Log Converter . |
| [`IBusFilterBusCollection.Exists`](ibusfilterbuscollection-exists.md) | Checks in the Bus Log Converter whether a bus with a specific name already exists in the filtered bus collection. |
| [`IBusFilterBusCollection.GetIndex`](ibusfilterbuscollection-getindex.md) | Returns the index of a bus within the UsedBuses collection in the Bus Log Converter . |
| [`IBusFilterBusCollection.Item`](ibusfilterbuscollection-item.md) | Returns the bus that is associated with a specific index or name from a filtered bus collection, in the Bus Log Converter . |
| [`IBusFilterBusCollection.Move`](ibusfilterbuscollection-move.md) | Moves a bus in the UsedBuses collection to the specified position, in the Bus Log Converter . |
| [`IBusFilterBusCollection.Remove`](ibusfilterbuscollection-remove.md) | Deletes an element from the UsedBuses collection , in the Bus Log Converter . |
| [`IBusFilterBusCollection.RemoveAll`](ibusfilterbuscollection-removeall.md) | Deletes all elements from the UsedBuses collection , in the Bus Log Converter . |
| [`ICANConverter.Clear`](icanconverter-clear.md) | Deletes all settings of the Bus Log Converter . For compatibility, the Clear method sets the EnumSubstitution for ResultSettings property to True. Set this property to False if you want the Bus Log Converter to generate enumeration channels . |
| [`ICANConverter.Convert`](icanconverter-convert.md) | Converts logfiles into the TDM format. |
| [`ICANConverter.IsModified`](icanconverter-ismodified.md) | Specifies in the Bus Log Converter , whether the configuration of the Bus Log Converter has been modified. |
| [`ICANConverter.Load`](icanconverter-load.md) | Loads a file with the extension .tcc into the Bus Log Converter . TCC files contain all the saved settings that the Bus Log Converter requires. |
| [`ICANConverter.SaveAs`](icanconverter-saveas.md) | Saves all the settings of the Bus Log Converter in a file with the extension .tcc . |
| [`ICANConverter.ShowConvertDlg`](icanconverter-showconvertdlg.md) | Opens the Bus Log Converter dialog box, where you configure the conversion of logfiles to the TDM format. |
| [`IDbFileCollection.Add`](idbfilecollection-add.md) | Adds a database file to the DbFiles collection in the Bus Logfile Converter . |
| [`IDbFileCollection.Exists`](idbfilecollection-exists.md) | Checks in the Bus Log Converter whether a database file with a specific name already exists for a bus. |
| [`IDbFileCollection.GetIndex`](idbfilecollection-getindex.md) | Returns the index of a database file from the DbFiles collection in the Bus Log Converter . |
| [`IDbFileCollection.Item`](idbfilecollection-item.md) | Returns the database file that is associated with a specific index or name, in the Bus Log Converter . |
| [`IDbFileCollection.Move`](idbfilecollection-move.md) | Moves a database file in the DbFiles collection to the specified position, in the Bus Log Converter . |
| [`IDbFileCollection.Remove`](idbfilecollection-remove.md) | Deletes an element from the DbFiles collection , in the Bus Log Converter . |
| [`IDbFileCollection.RemoveAll`](idbfilecollection-removeall.md) | Deletes all database files from the DbFiles collection , in the Bus Log Converter . |
| [`ILogFileCollection.Add`](ilogfilecollection-add.md) | Adds a database file to the LogFiles collection in the Bus Logfile Converter . |
| [`ILogFileCollection.Exists`](ilogfilecollection-exists.md) | Checks in the Bus Log Converter whether a logfile file with a specific name already exists. |
| [`ILogFileCollection.GetIndex`](ilogfilecollection-getindex.md) | Returns the index of a logfile from the LogFiles collection in the Bus Log Converter . |
| [`ILogFileCollection.Item`](ilogfilecollection-item.md) | Returns the logfile that is associated with a specific index or name, in the Bus Log Converter . |
| [`ILogFileCollection.Move`](ilogfilecollection-move.md) | Moves a logfile in the LogFiles collection to a specified position, in the Bus Log Converter . |
| [`ILogFileCollection.Remove`](ilogfilecollection-remove.md) | Deletes an element from the LogFiles collection , in the Bus Log Converter . |
| [`ILogFileCollection.RemoveAll`](ilogfilecollection-removeall.md) | Deletes all elements from the LogFiles collection , in the Bus Log Converter . |
| [`ISignalFilter.Load`](isignalfilter-load.md) | Loads a filter definition in the Bus Log Converter with the filename extension *.tsd or *.txt . |
| [`ISignalFilter.SaveAs`](isignalfilter-saveas.md) | Saves the current filter definition of the Bus Log Converter with the filename extension *.tsd . |
| [`IToStringItemVecInt.Add`](itostringitemvecint-add.md) | Adds a text to the StringVector collection in the Bus Log Converter . |
| [`IToStringItemVecInt.Item`](itostringitemvecint-item.md) | Specifies in the Bus Log Converter text associated to a specific index. |
| [`IToStringItemVecInt.Remove`](itostringitemvecint-remove.md) | Deletes an element in the StringVector object in the Bus Log Converter . |
| [`IToStringItemVecInt.RemoveAll`](itostringitemvecint-removeall.md) | Deletes all elements in the StringVector object in the Bus Log Converter . |
| [`IToStringItemVecUniqueInt.Add`](itostringitemvecuniqueint-add.md) | Adds a text to the string vector containing the names of the signals by which the Bus Log Converter filters. |
| [`IToStringItemVecUniqueInt.Item`](itostringitemvecuniqueint-item.md) | Specifies in the Bus Log Converter filter text associated with a specific index. |
| [`IToStringItemVecUniqueInt.Remove`](itostringitemvecuniqueint-remove.md) | Deletes a text in the string vector containing the names of the signals by which the Bus Log Converter filters. |
| [`IToStringItemVecUniqueInt.RemoveAll`](itostringitemvecuniqueint-removeall.md) | Deletes all texts in the string vector containing the names of the signals by which the Bus Log Converter filters. |
