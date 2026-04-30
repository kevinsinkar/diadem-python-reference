---
title: "Objects (DataPlugin Authoring)"
---

# Objects

33 objects from `DataPlugin.chm`.

| Name | Summary |
| --- | --- |
| [`IAbstractChannel`](iabstractchannel.md) | The AbstractChannel object provides the channel values and the associated properties. The AbstractChannel object corresponds with a Channel , a DirectAccessChannel or an ImplicitChannel . |
| [`IAbstractChannelFormatter`](iabstractchannelformatter.md) | The AbstractChannelFormatter object contains information about how the values of a channel are represented in the file. |
| [`IAutoRemove`](iautoremove.md) | The AutoRemove object offers support when working with ZIP archives. The methods allow you to unzip ZIP archives to a temporary folder and automatically delete the files in this folder. Note that a ZIP archive contains exactly one measurement data file. The DataFinder indexes a ZIP file only once, like any other measurement data file. Addressing within the ZIP archive is not possible. |
| [`IBinaryBlock`](ibinaryblock.md) | Use the BinaryBlock object to access channel data from a binary file. |
| [`IBinaryChannelFormatter`](ibinarychannelformatter.md) | The BinaryChannelFormatter object contains information about how the values of a channel are represented in the binary file. |
| [`ICellBlock`](icellblock.md) | The CellBlock object makes accessing data in a workbook easier. A CellBlock can contain one or more DirectAccess channels. The channel values are organized columnwise in this block. You read the contents of a workbook as follows: - use the Workbook.GetCellBlock method and assign the return value to a variable. - add a DirectAccess channel to the CellBlock for each channel to be read, - assign the complete DirectAccess channel to a channel group. Note The file pointer of the worksheet does not move when a CellBlock is read out. |
| [`ICellChannelFormatter`](icellchannelformatter.md) | The CellChannelFormatter object contains information about how the values of a channel are represented in the workbook. |
| [`IChannel`](ichannel.md) | The Channel object provides the channel values and the associated properties. |
| [`IChannelGroup`](ichannelgroup.md) | The ChannelGroup object provides a channel group including the associated channels and properties. |
| [`IDataPlugin`](idataplugin.md) | The DataPlugin object is available as a global object. Therefore, all the properties and methods of the object are available at all points in the script. |
| [`IDirectAccessChannel`](idirectaccesschannel.md) | The DirectAccessChannel object provides access to a DirectAccess channel and the associated properties. |
| [`IDocumentNamespace`](idocumentnamespace.md) | The DocumentNamespace <DataPlugin> object provides the namespace in a document. Use namespaces to group XML elements in a document. |
| [`IDocumentProperty`](idocumentproperty.md) | The DocumentProperty <DataPlugin> object provides a document's meta property. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IDocumentRoot`](idocumentroot.md) | The Document <DataPlugin> object provides the properties and methods for accessing the meta properties of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file. |
| [`IExcelFileIO`](iexcelfileio.md) | The Workbook object provides a workbook and the associated properties. |
| [`IExcelFormatter`](iexcelformatter.md) | The CellFormatter object contains information about the format of the workbook that the DataPlugin is currently processing. |
| [`IExcelPosition`](iexcelposition.md) | The CellPosition object provides the column and the row of a cell in a worksheet. |
| [`IExcelSheet`](iexcelsheet.md) | The Sheet object provides a worksheet from the open work folder and the associated properties. |
| [`IFileInfo`](ifileinfo.md) | The Info object contains information about the file that the DataPlugin is currently processing. |
| [`IFixedWidthBlock`](ifixedwidthblock.md) | Use the FixedWidthBlock object to access channel data in a text file. |
| [`IFixedWidthChannelFormatter`](ifixedwidthchannelformatter.md) | The FixedWidthChannelFormatter object contains information about how the values of a channel are represented in the text file. |
| [`IFormatter`](iformatter.md) | The Formatter object contains information about the format of the file that the DataPlugin is currently processing. |
| [`IImplicitChannel`](iimplicitchannel.md) | The ImplicitChannel object provides an implicit channel and the associated properties. |
| [`IMeasurementFileIO`](imeasurementfileio.md) | The File object provides information such as the name, origin, and size of the file the DataPlugin is currently processing. You use the File object properties to specify the special format of this file. The file is either a text file or a binary file. Use the methods of the File object to access this file. You can use the methods to read single values, texts, or sections from the file. |
| [`IProcessedChannel`](iprocessedchannel.md) | The ProcessedChannel object provides a channel, which combines values from other channels ( ChannelsToProcess ), and the associated properties. |
| [`IProperty`](iproperty.md) | The Property object provides a property for the Root object, for the ChannelGroup object, or for the Channel object. This property is either a base property of the data model, or a user-defined custom property. |
| [`IRoot`](iroot.md) | The Root object provides the list of all channel groups and all properties of the data set. |
| [`IStringBlock`](istringblock.md) | The StringBlock object facilitates access to text, single values, and channel data in a text file. |
| [`IStringChannelFormatter`](istringchannelformatter.md) | The StringChannelFormatter object contains information about how the values of a channel are represented in the text file. |
| [`IUSIElement`](iusielement.md) | The Element object contains information about the currently edited data store. |
| [`IUSISimplifiedStore`](iusisimplifiedstore.md) | The Store object provides information on the data store currently processed by the DataPlugin. Use the Store object properties to specify how to map the information about a data model, for example, ATFX files, onto the TDM data model. You also can use the Store object to change, to rename, or to extend information about a TDM data model. |
| [`IUsiTimeDisp`](iusitimedisp.md) | The USITimeDisp object provides date and time information. |
| [`IWorkbookInfo`](iworkbookinfo.md) | The WorkbookInfo object provides information on the open workbook. |
