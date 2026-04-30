---
title: "Properties (ICANConverter)"
---

# Properties

41 properties from `ICANConverter.chm`.

| Name | Summary |
| --- | --- |
| [`IBus.DbFiles`](ibus-dbfiles.md) | Returns the database files that are associated with a bus in the Bus Log Converter . You cannot overwrite the DbFiles property. |
| [`IBus.Name`](ibus-name.md) | Specifies the name of a bus in the Bus Log Converter . |
| [`IBus.Number`](ibus-number.md) | Specifies the number of a bus in the Bus Log Converter . You cannot overwrite the Number property. |
| [`IBus.Type`](ibus-type.md) | Specifies the type of a bus in the Bus Log Converter . You cannot overwrite the Type property. |
| [`IBusCollection.Count`](ibuscollection-count.md) | Specifies the number of buses to be converted in the Bus Log Converter . You cannot overwrite the Count property. |
| [`IBusDbConfig.Buses`](ibusdbconfig-buses.md) | Returns all the buses that are referenced in the logfiles, in the Bus Log Converter . You cannot overwrite the Buses property. |
| [`IBusDbConfig.Description`](ibusdbconfig-description.md) | Returns the description of a bus database configuration in the Bus Log Converter . |
| [`IBusDbConfig.Name`](ibusdbconfig-name.md) | Specifies the name of a bus database configuration in the Bus Log Converter . |
| [`IBusFilter.Active`](ibusfilter-active.md) | Specifies whether the filter, which converts only specific buses in the logfiles and not all the buses that are referenced in the logfiles, is active in the Bus Log Converter . |
| [`IBusFilter.UsedBuses`](ibusfilter-usedbuses.md) | Returns in the Bus Log Converter all buses the Bus Log Converter converts when the filter is active. You cannot overwrite the UsedBuses property. |
| [`IBusFilterBusCollection.Count`](ibusfilterbuscollection-count.md) | Specifies the number of buses that the Bus Log Converter still converts when the filter is active, in the Bus Log Converter . You cannot overwrite the Count property. |
| [`ICANConverter.BusDbConfig`](icanconverter-busdbconfig.md) | Specifies the configuration of buses and the associated database files in the Bus Log Converter . You cannot overwrite the BusDbConfig property. |
| [`ICANConverter.FileName`](icanconverter-filename.md) | Returns in the Bus Log Converter the filename of the file that contains the Bus Log Converter settings. You cannot overwrite the FileName property. |
| [`ICANConverter.LogSettings`](icanconverter-logsettings.md) | Specifies in the Bus Log Converter the logfiles to be converted and the type of these logfiles. You cannot overwrite the LogSettings property. |
| [`ICANConverter.ResultSettings`](icanconverter-resultsettings.md) | Returns the settings for the conversion results in the Bus Log Converter . You cannot overwrite the ResultSettings property. |
| [`IDbFile.Clusters`](idbfile-clusters.md) | Specifies one or several clusters in a Fibex database file in the Bus Log Converter . |
| [`IDbFile.DisplayFile`](idbfile-displayfile.md) | Specifies in the Bus Log Converter the name of a database file that belongs to a specific bus. The DisplayFile property is write-protected and does not contain the file path. |
| [`IDbFile.File`](idbfile-file.md) | Specifies the name and the path of a database file that is associated with a specific bus in the Bus Log Converter . |
| [`IDbFile.IdMode`](idbfile-idmode.md) | Specifies in the Bus Log Converter whether the database file is a standard file or a file with a special mode. |
| [`IDbFileCollection.Count`](idbfilecollection-count.md) | Specifies in the Bus Log Converter the number of database files which are assigned to a specific bus. You cannot overwrite the Count property. |
| [`ILogFile.DisplayFile`](ilogfile-displayfile.md) | Specifies the name of a logfile in the Bus Log Converter . The DisplayFile property does not contain the file path. You cannot overwrite the DisplayFile property. |
| [`ILogFile.File`](ilogfile-file.md) | Specifies the name and the path of a logfile in the Bus Log Converter . |
| [`ILogFile.XnetTdmsChannels`](ilogfile-xnettdmschannels.md) | Specifies in the Bus Log Converter the names of the channels to be converted in an NI-XNET-TDMS logfile. Only use this property for TDMS logfiles. If you do not assign channels to this property so that the string is empty, DIAdem converts all channels in the TDMS logfile. |
| [`ILogFileCollection.Count`](ilogfilecollection-count.md) | Specifies the number of logfiles to be converted in the Bus Log Converter . You can enter multiple logfiles in GIN-Multilogger files, but only one logfile in all other formats. You cannot overwrite the Count property. |
| [`ILogSettings.FileType`](ilogsettings-filetype.md) | Specifies in the Bus Log Converter the file type of the logfile to be converted. The file type eLogFileTypeTTL is a preview feature and can only be used in the Bus Log Converter if you have enabled the corresponding preview feature. Preview features are new developments that will be available as a full feature in one of the upcoming DIAdem versions. The user interface, the API, and the scope of functions is subject to change. |
| [`ILogSettings.LogFiles`](ilogsettings-logfiles.md) | Returns all the logfiles that are selected for conversion in the Bus Log Converter . You can only specify several logfiles for GIN-Multilogger files. You cannot overwrite the LogFiles property. |
| [`IResultSettings.BusFilter`](iresultsettings-busfilter.md) | Specifies the settings for the bus filter in the Bus Log Converter . You cannot overwrite the BusFilter property. |
| [`IResultSettings.EnumSubstitution`](iresultsettings-enumsubstitution.md) | Specifies whether the Bus Log Converter replaces enumeration strings of a logfile that is to be converted in the data channel of the TDM file, by NoValues or generates enumeration channels . |
| [`IResultSettings.NumberOfSkippedFrames`](iresultsettings-numberofskippedframes.md) | Specifies the number of frames at the beginning, which the Bus Log Converter ignores when converting. |
| [`IResultSettings.ResultFile`](iresultsettings-resultfile.md) | Specifies the name and the path of the TDM file into which the CAN Converter converts the selected logfiles in the Bus Log Converter . |
| [`IResultSettings.SequenceChannel`](iresultsettings-sequencechannel.md) | Specifies whether the Bus Log Converter generates an additional channel with the order of the telegrams in the Bus Log Converter for each channel group. |
| [`IResultSettings.SignalFilter`](iresultsettings-signalfilter.md) | Returns the SignalFilter object. The SignalFilter object provides a filter for the Bus Log Converter . If the Active property has the value TRUE , the Bus Log Converter loads only the signal names (upper or lower case) that are in the filter list. |
| [`IResultSettings.SkipFirstFrames`](iresultsettings-skipfirstframes.md) | Specifies that the Bus Log Converter ignores the first frames when converting. |
| [`IResultSettings.TimeFilter`](iresultsettings-timefilter.md) | Returns the settings for the time channels in the Bus Log Converter . You cannot overwrite the TimeFilter property. |
| [`ISignalFilter.Active`](isignalfilter-active.md) | Specifies whether a filter is enabled for the Bus Log Converter . When a filter is enabled, the Bus Log Converter only loads the signals (upper and lowercase) that are in the filter list. |
| [`ISignalFilter.Signals`](isignalfilter-signals.md) | Specifies a string vector containing the names of the signals by which the Bus Log Converter filters. If the Active property has the value TRUE , the Bus Log Converter loads only the files (upper or lower case) that are in the filter list. |
| [`ITimeFilter.Active`](itimefilter-active.md) | Specifies whether a filter for the time channels is active in the Bus Log Converter . |
| [`ITimeFilter.Begin`](itimefilter-begin.md) | Specifies the start value for the time filter in seconds in the Bus Log Converter . The time filter specifies the section of the logfile which you can convert into the TDM file. Use the End property to specify the end value of the time filter. |
| [`ITimeFilter.End`](itimefilter-end.md) | Specifies the end value for the time filter in seconds in the Bus Log Converter . The time filter specifies the section of the logfile which you can convert into the TDM file. Use the Begin property to specify the start value of the time filter. |
| [`IToStringItemVecInt.Count`](itostringitemvecint-count.md) | Counts the clusters or XNET channels contained in a string vector in the Bus Log Converter . |
| [`IToStringItemVecUniqueInt.Count`](itostringitemvecuniqueint-count.md) | Returns the number of texts in the string vector containing the names of the signals by which the Bus Log Converter filters. |
