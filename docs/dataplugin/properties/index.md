---
title: "Properties (DataPlugin Authoring)"
---

# Properties

164 properties from `DataPlugin.chm`.

| Name | Summary |
| --- | --- |
| [`IAbstractChannel.DataType`](iabstractchannel-datatype.md) | Returns the data type of a channel. |
| [`IAbstractChannel.Name`](iabstractchannel-name.md) | Specifies a channel name. |
| [`IAbstractChannel.Properties`](iabstractchannel-properties.md) | Contains the Properties collection associated with a channel. |
| [`IAbstractDirectAccessChannels.Count`](iabstractdirectaccesschannels-count.md) | Returns the number of elements of a DirectAccessChannels or of a BinaryDirectAccessChannels collection. |
| [`IBinaryBlock.BlockLength`](ibinaryblock-blocklength.md) | Specifies the number of values that a channel in the BinaryBlock contains. If the number is -1 , the block extends to the end of the file. |
| [`IBinaryBlock.BlockWidth`](ibinaryblock-blockwidth.md) | Specifies the number of bytes between two consecutive values of a block channel. |
| [`IBinaryBlock.Channels`](ibinaryblock-channels.md) | Contains the DirectAccessChannels collection associated with a BinaryBlock object. |
| [`IBinaryBlock.Position`](ibinaryblock-position.md) | Specifies the position of the file pointer in a BinaryBlock. |
| [`IBinaryChannelFormatter.BitMask`](ibinarychannelformatter-bitmask.md) | Specifies the bit mask that masks the value DIAdem reads in. |
| [`IBinaryChannelFormatter.Block`](ibinarychannelformatter-block.md) | Contains the parent object for a BinaryChannelFormatter object. |
| [`IBinaryChannelFormatter.ByteOrder`](ibinarychannelformatter-byteorder.md) | Specifies the byte order for a channel in the file if the data type consists of several bytes. |
| [`IBinaryChannelFormatter.Datatype`](ibinarychannelformatter-datatype.md) | Specifies the data type of a DirectAccess channel that is associated with a BinaryBlock. |
| [`IBinaryDirectAccessChannels.Count`](ibinarydirectaccesschannels-count.md) | Returns the number of elements in a BinaryDirectAccessChannels collection. |
| [`ICellBlock.BlockLength`](icellblock-blocklength.md) | Specifies the number of values that a channel in the CellBlock contains. If the number is -1 , the block extends to the end of the file. |
| [`ICellBlock.Channels`](icellblock-channels.md) | Contains the DirectAccessChannels collection associated with a CellBlock object. |
| [`ICellBlock.Position`](icellblock-position.md) | Specifies the position of the file pointer in a CellBlock. |
| [`ICellChannelFormatter.Block`](icellchannelformatter-block.md) | Contains the parent object for a CellChannelFormatter object. |
| [`ICellChannelFormatter.DataType`](icellchannelformatter-datatype.md) | Specifies the data type of a DirectAccess channel that is associated with a CellBlock. |
| [`IChannel.ChannelGroup`](ichannel-channelgroup.md) | Specifies the channel group to which a channel is assigned. |
| [`IChannel.DataType`](ichannel-datatype.md) | Returns the data type of a channel. |
| [`IChannel.Factor`](ichannel-factor.md) | Specifies the factor that the read value is multiplied by. |
| [`IChannel.Name`](ichannel-name.md) | Receives the name of a Channel object. |
| [`IChannel.Offset`](ichannel-offset.md) | Specifies the offset that is added when a value is read. |
| [`IChannel.Properties`](ichannel-properties.md) | Contains the Properties collection associated with a Channel object. |
| [`IChannel.ReservedSize`](ichannel-reservedsize.md) | Specifies the number of values that are reserved for a channel. |
| [`IChannel.Size`](ichannel-size.md) | Returns the current number of values in a channel. |
| [`IChannel.Values`](ichannel-values.md) | Contains the single value of a channel at a specific channel position. |
| [`IChannelGroup.Channels`](ichannelgroup-channels.md) | Contains the Channels collection associated with a ChannelGroup object. |
| [`IChannelGroup.Name`](ichannelgroup-name.md) | Receives the name of a ChannelGroup object. |
| [`IChannelGroup.Properties`](ichannelgroup-properties.md) | Contains the Properties collection associated with a ChannelGroup object. |
| [`IChannelGroup.Root`](ichannelgroup-root.md) | Contains the parent object associated with a ChannelGroup object. |
| [`IChannelGroups.Count`](ichannelgroups-count.md) | Returns the number of elements in a ChannelGroups collection. |
| [`IChannels.Count`](ichannels-count.md) | Returns the number of elements in a Channels collection. |
| [`IChannelsToProcess.Count`](ichannelstoprocess-count.md) | Returns the number of elements in a ChannelsToProcess collection. |
| [`IDataPlugin.AutoRemove`](idataplugin-autoremove.md) | Returns the AutoRemove object for working with ZIP archives. |
| [`IDataPlugin.CurrentScriptName`](idataplugin-currentscriptname.md) | Specifies the name of the script file which belongs to the currently executed DataPlugin. |
| [`IDataPlugin.CurrentScriptPath`](idataplugin-currentscriptpath.md) | Specifies the path of the script file which belongs to the currently executed DataPlugin. |
| [`IDataPlugin.Root`](idataplugin-root.md) | Contains the collection of all the channel groups and all the properties of the data set |
| [`IDirectAccessChannel.DataType`](idirectaccesschannel-datatype.md) | Specifies the data type of a DirectAccessChannel. |
| [`IDirectAccessChannel.Factor`](idirectaccesschannel-factor.md) | Specifies the factor that the read value is multiplied by. |
| [`IDirectAccessChannel.Formatter`](idirectaccesschannel-formatter.md) | Contains information about how the values of a DirectAccess channel are represented. |
| [`IDirectAccessChannel.Index`](idirectaccesschannel-index.md) | Specifies the position of the DirectAccess channel in the block. |
| [`IDirectAccessChannel.Name`](idirectaccesschannel-name.md) | Specifies the name of a DirectAccessChannel object. |
| [`IDirectAccessChannel.Offset`](idirectaccesschannel-offset.md) | Specifies the offset that is added when a value is read. |
| [`IDirectAccessChannel.Properties`](idirectaccesschannel-properties.md) | Contains the Properties collection associated with a DirectAccess channel. |
| [`IDirectAccessChannel.Size`](idirectaccesschannel-size.md) | Returns the current number of values in a DirectAccess channel. |
| [`IDirectAccessChannel.Values`](idirectaccesschannel-values.md) | Returns the single value of a DirectAccessChannel at a specific channel position. |
| [`IDirectAccessChannels.Count`](idirectaccesschannels-count.md) | Returns the number of elements in a DirectAccessChannels collection. |
| [`IDocumentNamespace.Name`](idocumentnamespace-name.md) | Returns the name of a namespace in a document. Use namespaces to group XML elements in a document. |
| [`IDocumentNamespace.Properties`](idocumentnamespace-properties.md) | Returns all meta properties in a specific namespace of a document. Use namespaces to identify XML elements clearly in a document. |
| [`IDocumentNamespaces.Count`](idocumentnamespaces-count.md) | Returns the number of namespaces of a document. Use namespaces to group XML elements in a document. |
| [`IDocumentProperty.Custom`](idocumentproperty-custom.md) | Specifies whether a meta property of a document is a custom property. Custom properties are user-defined meta properties of a document. A document can be an Office file in XML format, a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentProperty.DataType`](idocumentproperty-datatype.md) | Returns the data type of a meta property of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentProperty.Name`](idocumentproperty-name.md) | Returns the name of a meta property of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentProperty.Value`](idocumentproperty-value.md) | Specifies the value of a meta property of a document.  A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentReadProperties.Count`](idocumentreadproperties-count.md) | Returns the number of meta properties of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentRoot.FilePath`](idocumentroot-filepath.md) | Returns the absolute path of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentRoot.FileType`](idocumentroot-filetype.md) | Returns the data type of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. |
| [`IDocumentRoot.Namespaces`](idocumentroot-namespaces.md) | Returns all namespaces of a document. Use namespaces to identify groups of XML elements in a document. |
| [`IDocumentRoot.Properties`](idocumentroot-properties.md) | Returns all meta properties of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IExcelDAChannels.Count`](iexceldachannels-count.md) | Returns the number of elements in a DirectCellChannels collection. |
| [`IExcelFileIO.FileInfo`](iexcelfileio-fileinfo.md) | Returns the FileInfo object that contains information about the workbook that the DataPlugin is currently processing. |
| [`IExcelFileIO.Formatter`](iexcelfileio-formatter.md) | Returns the Formatter object that contains information about the format of the workbook that the DataPlugin is currently processing. |
| [`IExcelFileIO.Sheets`](iexcelfileio-sheets.md) | Returns a collection of the worksheets of a workbook. |
| [`IExcelFileIO.WorkbookInfo`](iexcelfileio-workbookinfo.md) | Returns the WorkbookInfo object that contains information about the workbook that the DataPlugin is currently processing. |
| [`IExcelFormatter.NoValueSign`](iexcelformatter-novaluesign.md) | Specifies the NoValue character used in the workbook. |
| [`IExcelFormatter.TimeFormat`](iexcelformatter-timeformat.md) | Specifies the time format used in the workbook. |
| [`IExcelPosition.Column`](iexcelposition-column.md) | Specifies the column number of a cell in a worksheet. |
| [`IExcelPosition.Row`](iexcelposition-row.md) | Specifies the row number of a cell in a worksheet. |
| [`IExcelSheet.Index`](iexcelsheet-index.md) | Specifies the position of the worksheet in the workbook. |
| [`IExcelSheet.MaxPosition`](iexcelsheet-maxposition.md) | Specifies within the worksheet the position of the cell that contains the last value. |
| [`IExcelSheet.MinPosition`](iexcelsheet-minposition.md) | Specifies within the worksheet the position of the cell that contains the first value. |
| [`IExcelSheet.Name`](iexcelsheet-name.md) | Specifies the name of the worksheet. |
| [`IExcelSheets.Count`](iexcelsheets-count.md) | Returns the number of worksheets in a workbook. |
| [`IFileInfo.Directory`](ifileinfo-directory.md) | Returns the folder of the processed file. |
| [`IFileInfo.Drive`](ifileinfo-drive.md) | Returns the drive letter of the processed file. |
| [`IFileInfo.Extension`](ifileinfo-extension.md) | Returns the filename extension of the processed file. |
| [`IFileInfo.FileName`](ifileinfo-filename.md) | Returns the name of the processed file. |
| [`IFileInfo.FullPath`](ifileinfo-fullpath.md) | Returns the name of the processed file, including the filename extension, and the path. |
| [`IFixedWidthBlock.BlockLength`](ifixedwidthblock-blocklength.md) | Specifies the number of values that a channel in the FixedWidthBlock contains. If the number is -1 , the block extends to the end of the file. |
| [`IFixedWidthBlock.Channels`](ifixedwidthblock-channels.md) | Contains the DirectAccessChannels collection associated with a FixedWidthBlock object. |
| [`IFixedWidthBlock.Position`](ifixedwidthblock-position.md) | Specifies the position of the file pointer in a FixedWidthBlock. |
| [`IFixedWidthChannelFormatter.Block`](ifixedwidthchannelformatter-block.md) | Contains the parent object for a FixedWidthChannelFormatter object. |
| [`IFixedWidthChannelFormatter.CharacterCount`](ifixedwidthchannelformatter-charactercount.md) | Specifies the number of characters that are read from the text file per channel value. The default value for this property is 10. |
| [`IFixedWidthChannelFormatter.Datatype`](ifixedwidthchannelformatter-datatype.md) | Specifies the data type of a DirectAccess channel that is associated with a FixedWidthBlock. |
| [`IFixedWidthChannelFormatter.SampleWidth`](ifixedwidthchannelformatter-samplewidth.md) | Specifies how many consecutive values are read from a line in the text file for one channel. The default value for this property is 1. |
| [`IFormatter.ByteOrder`](iformatter-byteorder.md) | Specifies the byte order in the file if the data type consists of several bytes. |
| [`IFormatter.CharacterFormat`](iformatter-characterformat.md) | Specifies the coding for interpreting the strings in the file. |
| [`IFormatter.CommentSign`](iformatter-commentsign.md) | Specifies the characters that mark comment lines in the file. These characters must be at the start of the line. |
| [`IFormatter.DecimalPoint`](iformatter-decimalpoint.md) | Specifies the decimal symbol used in the file. |
| [`IFormatter.Delimiters`](iformatter-delimiters.md) | Specifies the characters that separate values or text in the file. |
| [`IFormatter.ExponentSeparator`](iformatter-exponentseparator.md) | Specifies the exponential character used in the file. |
| [`IFormatter.IgnoreEmptyLines`](iformatter-ignoreemptylines.md) | Specifies whether the empty lines in the file are ignored. |
| [`IFormatter.LineFeeds`](iformatter-linefeeds.md) | Specifies the characters that indicate the line ends in the file. Use the GetLineFeed for File method to automatically determine the end of line character of a file. |
| [`IFormatter.NoValueSign`](iformatter-novaluesign.md) | Specifies the NoValue character used in the file. |
| [`IFormatter.StringSign`](iformatter-stringsign.md) | Specifies the character that identifies the beginning and the end of a text. The text identifier is ignored when the text is read. Text between two text identifiers are not interpreted when text is read. |
| [`IFormatter.ThousandSeparator`](iformatter-thousandseparator.md) | Specifies the thousands separator, which is ignored when values are read in. |
| [`IFormatter.TimeFormat`](iformatter-timeformat.md) | Specifies the format for the time values in the file. |
| [`IFormatter.TrimCharacters`](iformatter-trimcharacters.md) | Specifies the characters that are deleted before and after a value when it is read in. |
| [`IImplicitChannel.ChannelGroup`](iimplicitchannel-channelgroup.md) | Specifies the channel group to which the implicit channel is assigned. |
| [`IImplicitChannel.DataType`](iimplicitchannel-datatype.md) | Specifies the data type of an implicit channel. |
| [`IImplicitChannel.Increment`](iimplicitchannel-increment.md) | Specifies the step width for generating the data of an implicit channel. |
| [`IImplicitChannel.Name`](iimplicitchannel-name.md) | Receives the name of an ImplicitChannel object. |
| [`IImplicitChannel.Properties`](iimplicitchannel-properties.md) | Contains the Properties collection associated with an implicit channel. |
| [`IImplicitChannel.Size`](iimplicitchannel-size.md) | Specifies the number of values of an implicit channel. |
| [`IImplicitChannel.StartValue`](iimplicitchannel-startvalue.md) | Specifies the start value for generating the data of an implicit channel. |
| [`IImplicitChannel.Values`](iimplicitchannel-values.md) | Contains the single value of a channel at a specific channel position. |
| [`IMeasurementFileIO.Formatter`](imeasurementfileio-formatter.md) | Returns the Formatter object that contains information about the format of the file that the DataPlugin is currently processing. |
| [`IMeasurementFileIO.Info`](imeasurementfileio-info.md) | Returns the Info object that contains information about the file that the DataPlugin is currently processing. |
| [`IMeasurementFileIO.Position`](imeasurementfileio-position.md) | Specifies the current position of the file pointer. |
| [`IMeasurementFileIO.Size`](imeasurementfileio-size.md) | Returns the current size of the file in bytes. |
| [`IProcessedChannel.ChannelGroup`](iprocessedchannel-channelgroup.md) | Specifies the channel group to which the ProcessedChannel channel type is assigned. |
| [`IProcessedChannel.Channels`](iprocessedchannel-channels.md) | Contains the ChannelsToProcess collection associated with a ProcessedChannel object. |
| [`IProcessedChannel.DataType`](iprocessedchannel-datatype.md) | Returns the data type of a channel. |
| [`IProcessedChannel.Factor`](iprocessedchannel-factor.md) | Specifies the factor that the read value is multiplied by. |
| [`IProcessedChannel.Name`](iprocessedchannel-name.md) | Receives the name of a ProcessedChannel object. |
| [`IProcessedChannel.Offset`](iprocessedchannel-offset.md) | Specifies the offset that is added when a value is read. |
| [`IProcessedChannel.Properties`](iprocessedchannel-properties.md) | Contains the Properties collection associated with a ProcessedChannel object. |
| [`IProcessedChannel.Size`](iprocessedchannel-size.md) | Returns the current number of values in a channel. |
| [`IProcessedChannel.Values`](iprocessedchannel-values.md) | Returns the single value of a Channel at a specific channel position. |
| [`IProperties.Count`](iproperties-count.md) | Returns the number of elements in a Properties collection. |
| [`IProperty.DataType`](iproperty-datatype.md) | Specifies the data type of a property or of a custom property. |
| [`IProperty.Default`](iproperty-default.md) | Specifies whether a property is a base property . |
| [`IProperty.Name`](iproperty-name.md) | Returns the name of a Property object. |
| [`IProperty.Size`](iproperty-size.md) | Specifies the number of values of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object. |
| [`IProperty.Value`](iproperty-value.md) | Specifies the value of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object. |
| [`IProperty.Values`](iproperty-values.md) | Specifies a vector with values of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object. The size of the vector depends on the Size property. |
| [`IRoot.ChannelGroups`](iroot-channelgroups.md) | Contains the ChannelGroups collection associated with a Root object. |
| [`IRoot.Name`](iroot-name.md) | Specifies the name of the Root object. The Data Portal displays this name in the Source name property after loading the data. |
| [`IRoot.Properties`](iroot-properties.md) | Contains the Properties collection associated with a Root object. |
| [`IStringBlock.BlockLength`](istringblock-blocklength.md) | Specifies the number of values that a channel in the StringBlock contains. If the number is -1 , the block extends to the end of the file. |
| [`IStringBlock.Channels`](istringblock-channels.md) | Contains the DirectAccessChannels collection associated with a StringBlock object. |
| [`IStringBlock.Position`](istringblock-position.md) | Specifies the position of the file pointer in a StringBlock. |
| [`IStringChannelFormatter.Block`](istringchannelformatter-block.md) | Contains the parent object for a StringChannelFormatter object. |
| [`IStringChannelFormatter.Datatype`](istringchannelformatter-datatype.md) | Specifies the data type of a DirectAccess channel that is associated with a StringBlock. |
| [`IStringChannelFormatter.DecimalPoint`](istringchannelformatter-decimalpoint.md) | Specifies the decimal symbol used in a channel. |
| [`IStringChannelFormatter.NoValueSign`](istringchannelformatter-novaluesign.md) | Specifies the NoValue character used in a channel. |
| [`IStringChannelFormatter.ThousandSeparator`](istringchannelformatter-thousandseparator.md) | Specifies the thousands separator, which is ignored when channel values are read in. |
| [`IStringChannelFormatter.TimeFormat`](istringchannelformatter-timeformat.md) | Specifies the format for the channel time values in the file. |
| [`IUSIElement.Children`](iusielement-children.md) | Contains the StoreElements collection associated with an Element object. |
| [`IUSIElement.Name`](iusielement-name.md) | Receives the name of an Element object. |
| [`IUSIElement.Properties`](iusielement-properties.md) | Contains the Properties collection associated with an Element object. |
| [`IUSIElement.Type`](iusielement-type.md) | Returns the type of an Element object. |
| [`IUSIElements.Count`](iusielements-count.md) | Returns the number of elements in a Elements collection. |
| [`IUSISimplifiedStore.Children`](iusisimplifiedstore-children.md) | Contains the StoreElements collection associated with a Store object. |
| [`IUSISimplifiedStore.ConfigFileName`](iusisimplifiedstore-configfilename.md) | Specifies the configuration file with the extension .stp , which contains the search path to be used. |
| [`IUSISimplifiedStore.FileInfo`](iusisimplifiedstore-fileinfo.md) | Returns the FileInfo object that contains information about the file that the DataPlugin is currently processing. |
| [`IUSISimplifiedStore.Parameters`](iusisimplifiedstore-parameters.md) | Specifies the name of a data file with the filename extension and the path. |
| [`IUSISimplifiedStore.PluginName`](iusisimplifiedstore-pluginname.md) | Contains the name of the DataPlugin that opens the data store. |
| [`IUsiTimeDisp.Day`](iusitimedisp-day.md) | Specifies the day. |
| [`IUsiTimeDisp.Fraction`](iusitimedisp-fraction.md) | Specifies in an USITimeDisp type object the fractions of a second with an accuracy of nanoseconds. |
| [`IUsiTimeDisp.Hour`](iusitimedisp-hour.md) | Specifies the hours. |
| [`IUsiTimeDisp.Microsecond`](iusitimedisp-microsecond.md) | Specifies the microseconds. |
| [`IUsiTimeDisp.Millisecond`](iusitimedisp-millisecond.md) | Specifies the milliseconds. |
| [`IUsiTimeDisp.Minute`](iusitimedisp-minute.md) | Specifies the minutes. |
| [`IUsiTimeDisp.Month`](iusitimedisp-month.md) | Specifies the month. |
| [`IUsiTimeDisp.Nanosecond`](iusitimedisp-nanosecond.md) | Specifies the nanoseconds. |
| [`IUsiTimeDisp.Second`](iusitimedisp-second.md) | Specifies the seconds. |
| [`IUsiTimeDisp.SecondsFrom0000`](iusitimedisp-secondsfrom0000.md) | Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 01/01/0000. |
| [`IUsiTimeDisp.SecondsFrom1904`](iusitimedisp-secondsfrom1904.md) | Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 1/1/1904. |
| [`IUsiTimeDisp.VariantDate`](iusitimedisp-variantdate.md) | Specifies a date or time. This entry does not include microseconds and nanoseconds. |
| [`IUsiTimeDisp.Year`](iusitimedisp-year.md) | Specifies the year. |
| [`IWorkbookInfo.Author`](iworkbookinfo-author.md) | Specifies the author of the edited workbook. |
| [`IWorkbookInfo.Title`](iworkbookinfo-title.md) | Specifies the description of the edited workbook. |
