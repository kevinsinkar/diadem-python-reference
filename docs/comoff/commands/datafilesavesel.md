---
title: "DataFileSaveSel"
description: "Saves selected channels and their properties from the DIAdem Data Portal to a data file. DIAdem saves the groups and channels in the target file in the same str"
---

# DataFileSaveSel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileSaveSel

Saves selected channels and their properties from the DIAdem Data Portal to a data file. DIAdem saves the groups and channels in the target file in the same structure as in the Data Portal.

## Signature

```python
dd.DataFileSaveSel(DataFilename, FileExportFilter, SelectedChannels, [ ChnXYRelation ])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileExportFilter</span> variable for DataPlugins, enable the<a href="#" data-unresolved="1"> Recording mode</a> and select a file type in the <a href="#" data-unresolved="1">Save As</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../datafilesave/">DataFileSave</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not save data in the TDM format, group information or properties, for example, may be left out because some formats cannot save all information.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you save data in the CSV format, DIAdem saves only the first channel group. To save other channel groups, you must save the channel groups selectively.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you save data in the CSV format, DIAdem uses a tabulator as the separator.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you save data in TDM format, you use the <a href="../../../varoff/variables/filesavedatatype/">FileSaveDataType</a> variable to specify whether DIAdem specifies the data format automatically, or saves the data format as a floating point value with 64 bits. By default, DIAdem specifies the data format automatically.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The page <a href="#" data-unresolved="1">Loading Bulk Data - General</a> contains important information on the extended loading behavior of TDM and TDMS files.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DataFilename</td>
<td>Specifies the name of a data file with the filename extension and the path.<div id="exp_DataFilename">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
</div></td></tr>
<tr><td width="150">FileExportFilter</td>
<td>Specifies the storage method you use to save data from the DIAdem Data Portal to a file. If you do not specify a storage method, DIAdem saves the data with the TDM DataPlugin.<div id="exp_FileExportFilter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">The valid values for this variable vary according to the registered DataPlugin. The following values are valid:</p>
<table class="Borderless" width="590"><tr><td width="150"><strong>Value of the variable</strong></td><td width="175"><strong>Meaning</strong></td>
<td width="239"><strong>Filename extension</strong></td></tr><tr><td width="150"><span class="Monospace">TDM</span></td><td width="175">DIAdem TDM files</td>
<td width="239"><span class="Monospace">TDM</span></td></tr><tr><td width="150"><span class="Monospace">DD8x</span></td><td width="175">DIAdem DAT files</td>
<td width="239"><span class="Monospace">DAT</span></td></tr>
<tr>
<td width="150"><span class="Monospace">TDMS</span></td><td width="175">DIAdem TDM streaming files</td>
<td width="239"><span class="Monospace">TDMS</span></td></tr>
<tr><td width="150"><span class="Monospace">LVM</span></td><td width="175">LabVIEW LVM files</td>
<td width="239"><span class="Monospace">LVM</span></td></tr>
<tr>
<td width="150"><span class="Monospace">ATF</span></td><td width="175">ASAM transport format</td>
<td width="239"><span class="Monospace">ATF</span></td></tr>
<tr>
<td width="150"><span class="Monospace">CSV</span></td><td width="175">Comma-separated values</td>
<td width="239"><span class="Monospace">CSV</span></td></tr>
</table><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileExportFilter</span> variable for DataPlugins, enable the<a href="#" data-unresolved="1"> Recording mode</a> and select a file type in the <a href="#" data-unresolved="1">Save As</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../datafilesave/">DataFileSave</a> command.</td></tr></table><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not save data in the TDM format, group information or properties, for example, may be left out because some formats cannot save all information.</td></tr></table><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you save data in the CSV format, DIAdem saves only the first channel group. To save other channel groups, you must save the channel groups selectively.</td></tr></table><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you save data in the CSV format, DIAdem uses a tabulator as the separator.</td></tr></table>
</div></td></tr>
<tr><td width="150">SelectedChannels</td>
<td>Specifies the data channels that DIAdem saves in the target file. If you do not specify any channels, DIAdem saves all channels.<div id="exp_SelectedChannels">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">[ChnXYRelation]</td>
<td>Specifies that x-channel references are used when copying and moving xy-channels and are preserved during reduced loading of xy-channels.<div id="exp_ChnXYRelation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[1]/Channel*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
dd.DataFileSaveSel(dd.DataWritePath + "MyExample1.tdm", "TDM", oMyChannelList)
```

---

*Source: `ComOff/DataFileSaveSel.htm`*
