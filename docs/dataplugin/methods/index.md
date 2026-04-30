---
title: "Methods (DataPlugin Authoring)"
---

# Methods

104 methods from `DataPlugin.chm`.

| Name | Summary |
| --- | --- |
| [`IAbstractChannel.IsKindOf`](iabstractchannel-iskindof.md) | Checks whether a Channel object is a certain type. |
| [`IAbstractChannelFormatter.IsKindOf`](iabstractchannelformatter-iskindof.md) | Checks whether the AbstractChannelFormatter object is a certain type. The AbstractChannelFormatter object contains information about how the values of a channel are represented in the file. Depending on whether the channel belongs to a BinaryBlock, StringBlock, FixedWidthBlock, or CellBlock the AbstractChannelFormatter is a BinaryChannelFormatter , StringChannelFormatter , FixedWidthChannelFormatter , or CellChannelFormatter object. |
| [`IAbstractDirectAccessChannels.Item`](iabstractdirectaccesschannels-item.md) | Returns the DirectAccessChannel object associated with a specific name or with a specific index. |
| [`IAbstractDirectAccessChannels.Remove`](iabstractdirectaccesschannels-remove.md) | Deletes an element of the DirectAccessChannels collection or the BinaryDirectAccessChannels collection. |
| [`IAbstractDirectAccessChannels.RemoveAll`](iabstractdirectaccesschannels-removeall.md) | Deletes all the elements of the DirectAccessChannels collection or the BinaryDirectAccessChannels collection. |
| [`IAbstractDirectAccessChannels.Swap`](iabstractdirectaccesschannels-swap.md) | Moves a DirectAccess channel to a specific position. |
| [`IAutoRemove.AddExisting`](iautoremove-addexisting.md) | Reserves a file or a folder for deletion. The folder is deleted automatically, as soon as the DataPlugin has stopped importing the data. |
| [`IAutoRemove.CreateFolder`](iautoremove-createfolder.md) | Creates a new, unique folder reserved for the automatic deletion process. The automatic deletion of the folder and its files occurs as soon as the DataPlugin no longer requires these files. |
| [`IBinaryBlock.IsKindOf`](ibinaryblock-iskindof.md) | Checks whether a BinaryBlock object is a certain type. |
| [`IBinaryChannelFormatter.IsKindOf`](ibinarychannelformatter-iskindof.md) | Checks whether the BinaryChannelFormatter object is a certain type. |
| [`IBinaryDirectAccessChannels.Add`](ibinarydirectaccesschannels-add.md) | Adds an object to the Channels collection of a BinaryBlock and returns a DirectAccessChannel object. |
| [`IBinaryDirectAccessChannels.Item`](ibinarydirectaccesschannels-item.md) | Returns the DirectAccessChannel object associated with a specific name or with a specific index. |
| [`IBinaryDirectAccessChannels.Remove`](ibinarydirectaccesschannels-remove.md) | Deletes one element from the BinaryDirectAccessChannels collection. |
| [`IBinaryDirectAccessChannels.RemoveAll`](ibinarydirectaccesschannels-removeall.md) | Specifies all elements from the BinaryDirectAccessChannels collection. |
| [`IBinaryDirectAccessChannels.Swap`](ibinarydirectaccesschannels-swap.md) | Moves a DirectAccess channel to a specific position. |
| [`ICellChannelFormatter.IsKindOf`](icellchannelformatter-iskindof.md) | Checks whether the CellChannelFormatter object is a certain type. The CellChannelFormatter object contains information about how the values of a channel are represented in a workbook. The channel always belongs to a CellBlock . |
| [`IChannel.AddCharacteristics`](ichannel-addcharacteristics.md) | Specifies the characteristic values of a channel. |
| [`IChannel.AddWaveformProperties`](ichannel-addwaveformproperties.md) | Adds waveform properties to the channel to create a waveform channel. Waveform channels contain the x-part and the y-part of a curve in a channel. The y-part contains the (measurement) values. The x-part might be the measured time. The Waveform properties specify the x-part that is a linear specification with a start value and a step width. |
| [`IChannel.IsKindOf`](ichannel-iskindof.md) | Checks whether a Channel object is a certain type. |
| [`IChannelGroups.Add`](ichannelgroups-add.md) | Adds an object to the ChannelGroups collection and returns a ChannelGroup object. |
| [`IChannelGroups.Exists`](ichannelgroups-exists.md) | Checks whether a ChannelGroup object with a specific name exists. |
| [`IChannelGroups.Item`](ichannelgroups-item.md) | Returns the ChannelGroup object associated with a specific name or with a specific index. |
| [`IChannelGroups.Remove`](ichannelgroups-remove.md) | Deletes one element from the ChannelGroups collection. |
| [`IChannelGroups.RemoveAll`](ichannelgroups-removeall.md) | Deletes all elements from the ChannelGroups collection. |
| [`IChannels.Add`](ichannels-add.md) | Adds an object to the Channels collection and returns a Channel object. |
| [`IChannels.AddDirectAccessChannel`](ichannels-adddirectaccesschannel.md) | Adds an object to the Channels collection and returns a DirectAccessChannel object. |
| [`IChannels.AddImplicitChannel`](ichannels-addimplicitchannel.md) | Adds an object to the Channels collection and returns an ImplicitChannel object. |
| [`IChannels.AddProcessedChannel`](ichannels-addprocessedchannel.md) | Adds an object to the Channels collection and returns a ProcessedChannel object. |
| [`IChannels.AddStoreChannel`](ichannels-addstorechannel.md) | Adds an object to the Channels collection and returns an ImplicitChannel object or a ProcessedChannel object. |
| [`IChannels.Exists`](ichannels-exists.md) | Checks whether a Channel object with a specific name exists. |
| [`IChannels.Item`](ichannels-item.md) | Returns the Channel object associated with a specific name or with a specific index. |
| [`IChannels.Remove`](ichannels-remove.md) | Deletes one element from the Channels collection. |
| [`IChannels.RemoveAll`](ichannels-removeall.md) | Deletes all elements from the Channels collection. |
| [`IChannelsToProcess.Add`](ichannelstoprocess-add.md) | Adds an object to the ChannelsToProcess collection and returns a Channel object. |
| [`IChannelsToProcess.Item`](ichannelstoprocess-item.md) | Returns the Channel object of a specific index. |
| [`IChannelsToProcess.Remove`](ichannelstoprocess-remove.md) | Deletes one element from the ChannelsToProcess collection. |
| [`IChannelsToProcess.RemoveAll`](ichannelstoprocess-removeall.md) | Deletes all elements from the ChannelsToProcess collection. |
| [`IDataPlugin.CreateJsonParser`](idataplugin-createjsonparser.md) | Creates a JsonParser object with methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object or a VBS array , or vice versa. |
| [`IDataPlugin.CreateTime`](idataplugin-createtime.md) | Creates a time value. You can assign this time value to a value in a time channel or to a property. |
| [`IDataPlugin.DBM`](idataplugin-dbm.md) | Displays texts in a debug window. |
| [`IDataPlugin.OpenDocument`](idataplugin-opendocument.md) | Returns an object which provides methods and properties for reading or editing the metadata of a document. |
| [`IDataPlugin.OpenFile`](idataplugin-openfile.md) | Opens a file. |
| [`IDataPlugin.OpenSpreadsheet`](idataplugin-openspreadsheet.md) | Uses a specified DataPlugin to open an Excel file. To create this DataPlugin use the file reader Only filename in the Configure DataPlugin dialog box. The DataPlugin cannot access Excel files that are password protected. |
| [`IDataPlugin.OpenStore`](idataplugin-openstore.md) | Uses a specified DataPlugin to open a data store. |
| [`IDataPlugin.RaiseError`](idataplugin-raiseerror.md) | Aborts loading with an error message. |
| [`IDataPlugin.Unzip`](idataplugin-unzip.md) | Unzips a ZIP archive to a specified folder. The unzipped files are automatically deleted as soon as the DataPlugin no longer requires these files. |
| [`IDirectAccessChannel.AddCharacteristics`](idirectaccesschannel-addcharacteristics.md) | Specifies the characteristic values of a DirectAccessChannel. |
| [`IDirectAccessChannel.AddWaveformProperties`](idirectaccesschannel-addwaveformproperties.md) | Adds waveform properties to the DirectAccess channel to generate a waveform channel. Waveform channels contain the x-part and the y-part of a curve in a channel. The y-part contains the (measurement) values. The x-part might be the measured time. The Waveform properties specify the x-part that is a linear specification with a start value and a step width. |
| [`IDirectAccessChannel.IsKindOf`](idirectaccesschannel-iskindof.md) | Checks whether a DirectAccessChannel object is a certain type. |
| [`IDirectAccessChannels.Add`](idirectaccesschannels-add.md) | Adds an object to the Channels collection of a StringBlock, FixedWidthBlock, or a BinaryBlock and returns a DirectAccessChannel object. |
| [`IDirectAccessChannels.Item`](idirectaccesschannels-item.md) | Returns the DirectAccessChannel object associated with a specific name or with a specific index. |
| [`IDirectAccessChannels.Remove`](idirectaccesschannels-remove.md) | Deletes one element from the DirectAccessChannels collection. |
| [`IDirectAccessChannels.RemoveAll`](idirectaccesschannels-removeall.md) | Deletes all elements from the DirectAccessChannels collection. |
| [`IDirectAccessChannels.Swap`](idirectaccesschannels-swap.md) | Moves an DirectAccess channel to a specific position. |
| [`IDocumentNamespaces.Exists`](idocumentnamespaces-exists.md) | Specifies whether a namespace of a document already exists. Use namespaces to group XML elements in a document. |
| [`IDocumentNamespaces.Item`](idocumentnamespaces-item.md) | Returns a namespace of a document. Use namespaces to group XML elements in a document. |
| [`IDocumentReadProperties.Exists`](idocumentreadproperties-exists.md) | Checks whether a property with a specific name already exists in a document. A document can be an Office file in XML format, a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentReadProperties.Item`](idocumentreadproperties-item.md) | Returns a document's meta property not allocated to a namespace. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IExcelDAChannels.Add`](iexceldachannels-add.md) | Adds an object to the DirectCellChannels collection of a CellBlock and returns a DirectAccessChannel object. |
| [`IExcelDAChannels.Item`](iexceldachannels-item.md) | Returns the DirectAccessChannel object associated with a specific name or with a specific index. |
| [`IExcelDAChannels.Remove`](iexceldachannels-remove.md) | Deletes one element from the DirectCellChannels collection. |
| [`IExcelDAChannels.RemoveAll`](iexceldachannels-removeall.md) | Deletes all elements from the DirectCellChannels collection. |
| [`IExcelDAChannels.Swap`](iexceldachannels-swap.md) | Moves an DirectAccess channel to a specific position. |
| [`IExcelSheet.Find`](iexcelsheet-find.md) | Determines the position of a character or a character string in a worksheet of the open work folder. The search is executed rowwise. |
| [`IExcelSheet.GetCellBlock`](iexcelsheet-getcellblock.md) | Reads the worksheet starting at a specified position and returns the channel values the worksheet contains. |
| [`IExcelSheet.GetCellType`](iexcelsheet-getcelltype.md) | Returns the data type of worksheet cell. |
| [`IExcelSheet.GetCellValue`](iexcelsheet-getcellvalue.md) | Reads out the content of a worksheet cell. |
| [`IExcelSheets.Exists`](iexcelsheets-exists.md) | Checks whether a Sheet object with a specific name or index exists. |
| [`IExcelSheets.Item`](iexcelsheets-item.md) | Returns the Sheet object associated with a specific name or with a specific index. |
| [`IFixedWidthBlock.IsKindOf`](ifixedwidthblock-iskindof.md) | Checks whether a FixedWidthBlock object is a certain type. |
| [`IFixedWidthChannelFormatter.IsKindOf`](ifixedwidthchannelformatter-iskindof.md) | Checks whether a FixedWidthChannelFormatter object is a certain type. |
| [`IFormatter.ParseString`](iformatter-parsestring.md) | Parses a text into the specified data type. |
| [`IImplicitChannel.AddWaveformProperties`](iimplicitchannel-addwaveformproperties.md) | Adds waveform properties to the implicit channel to generate a waveform channel. Waveform channels contain the x-part and the y-part of a curve in a channel. The y-part contains the (measurement) values. The x-part might be the measured time. The Waveform properties specify the x-part that is a linear specification with a start value and a step width. |
| [`IImplicitChannel.IsKindOf`](iimplicitchannel-iskindof.md) | Checks whether a ImplicitChannel object is a certain type. |
| [`IMeasurementFileIO.GetBinaryBlock`](imeasurementfileio-getbinaryblock.md) | Reads a binary file and returns the channel values contained in the file. |
| [`IMeasurementFileIO.GetCharacters`](imeasurementfileio-getcharacters.md) | Reads a specific number of characters from the file. The method returns all characters, including delimiters and end of line characters. |
| [`IMeasurementFileIO.GetFixedWidthBlock`](imeasurementfileio-getfixedwidthblock.md) | Reads a text file and returns the channel values contained in the file. |
| [`IMeasurementFileIO.GetLineFeed`](imeasurementfileio-getlinefeed.md) | Determines the line end character in the file. |
| [`IMeasurementFileIO.GetNextBinaryValue`](imeasurementfileio-getnextbinaryvalue.md) | Reads a value at the current file position and moves the file pointer according to the data type of the value. |
| [`IMeasurementFileIO.GetNextLine`](imeasurementfileio-getnextline.md) | Reads all characters up to the next end of line. |
| [`IMeasurementFileIO.GetNextStringValue`](imeasurementfileio-getnextstringvalue.md) | Reads a value at the current file position and moves the file pointer according to the data type of the value. |
| [`IMeasurementFileIO.GetStringBlock`](imeasurementfileio-getstringblock.md) | Reads a text file and returns the channel values contained in the file. |
| [`IMeasurementFileIO.SkipLine`](imeasurementfileio-skipline.md) | Skips one line in the file. |
| [`IMeasurementFileIO.SkipLines`](imeasurementfileio-skiplines.md) | Skips several lines in the file. |
| [`IMeasurementFileIO.SkipValue`](imeasurementfileio-skipvalue.md) | Skips a value in a line. |
| [`IMeasurementFileIO.SkipValues`](imeasurementfileio-skipvalues.md) | Skips several values in a line. |
| [`IProcessedChannel.AddCharacteristics`](iprocessedchannel-addcharacteristics.md) | Specifies the characteristic values of a channel which combines the values from other channels ( ChannelsToProcess ). |
| [`IProcessedChannel.AddWaveformProperties`](iprocessedchannel-addwaveformproperties.md) | Adds waveform properties to a channel, which combines values form other channels ( ChannelsToProcess ), in order to create a waveform channel. Waveform channels contain the x-part and the y-part of a curve in a channel. The y-part contains the (measurement) values. The x-part might be the measured time. The Waveform properties specify the x-part that is a linear specification with a start value and a step width. |
| [`IProcessedChannel.IsKindOf`](iprocessedchannel-iskindof.md) | Checks whether a ProcessedChannel object is a certain type. |
| [`IProperties.Add`](iproperties-add.md) | Adds an object to the Properties collection and returns a Property object. |
| [`IProperties.AddProperties`](iproperties-addproperties.md) | Adds a list of properties to the Properties collection. |
| [`IProperties.Exists`](iproperties-exists.md) | Checks whether a Property object with a specific name exists. |
| [`IProperties.Item`](iproperties-item.md) | Returns the Property object associated with a specific name or with a specific index. |
| [`IProperties.Remove`](iproperties-remove.md) | Deletes one element from the Properties collection. |
| [`IProperties.RemoveAll`](iproperties-removeall.md) | Deletes all elements from the Properties collection. |
| [`IRoot.ImportStore`](iroot-importstore.md) | Imports a data file with a specified load method. You can only import data stores that are based on the TDM model. Note that you must not define any groups or properties for the Root object before calling this method. After importing the data file, you can use the Root object as usual. |
| [`IStringBlock.IsKindOf`](istringblock-iskindof.md) | Checks whether a StringBlock object is a certain type. |
| [`IStringChannelFormatter.IsKindOf`](istringchannelformatter-iskindof.md) | Checks whether a StringChannelFormatter object is a certain type. |
| [`IUSIElement.IsKindOf`](iusielement-iskindof.md) | Checks whether an Element object is a certain type. |
| [`IUSIElements.Item`](iusielements-item.md) | Returns the Element object of a specific index. |
| [`IUSIElements.Remove`](iusielements-remove.md) | Deletes one element from the Elements collection. |
| [`IUSIElements.RemoveAll`](iusielements-removeall.md) | Deletes all elements from the Elements collection. |
| [`IUsiTimeDisp.GetLocalTime`](iusitimedisp-getlocaltime.md) | Returns the time information saved in the USITimeDisp object as local time. The local time consists of a date and time specification. The GetLocalTime method does not execute a plausibility check and assumes that the time information to be converted is in UTC time. If this is not the case, the results are invalid. Therefore we recommend you know how local time is related to UTC time when you use this method. For example, UTC + 1 hour applies in Germany, which means 1 p. m. UTC is the same as 2 p.m. local time. During the daylight saving time, Germany adds a further hour to the UTC time. |
| [`IUsiTimeDisp.GetUTC`](iusitimedisp-getutc.md) | Returns the time information saved in the USITimeDisp object in coordinated world time as UTC time (Universal Time Coordinated). UTC time consists of a date and time specification. The GetUTC method does not execute a plausibility check and assumes that the time information to be converted is in local time. If this is not the case, the results are invalid. Therefore we recommend you know how local time is related to UTC time when you use this method. For example, UTC + 1 hour applies in Germany, which means 1 p. m. UTC is the same as 2 p.m. local time. During the daylight saving time, Germany adds a further hour to the UTC time. |
