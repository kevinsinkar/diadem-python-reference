---
title: "DataFileLoadSel"
description: "Loads selected channels from a data file into the DIAdem Data Portal."
---

# DataFileLoadSel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileLoadSel

Loads selected channels from a data file into the DIAdem Data Portal.

## Signature

```python
return_value = dd.DataFileLoadSel(DataFilename, FileImportFilter, ImportSelection, [ImportParameterSet])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileImportFilter</span> variable for a file type, enable the <a href="#" data-unresolved="1">Recording mode</a> and open a file with the appropriate filename extension in the <a href="#" data-unresolved="1">Open</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../datafileload/">DataFileLoad</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Visit the <a href="#">DataPlugin Website</a> to find existing DataPlugins you can download.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  Use the vertical separator |, to load channels from several channel groups, for example, <span class="Monospace">Call DataFileLoadSel("Example.tdm","TDM","[1]/[2]|[2]/[4]|[3]/[5]","Load")</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td>Note  If you are using the <span class="Monospace">ImportParameter</span> object for the <span class="Monospace">ImportParameterSet</span> variable, the <span class="Monospace">DataFileLoadSel</span> command supports the following properties: <a href="../../../scriptnavi/properties/iimportparameterset-importmode/">ImportMode</a>, <a href="../../../scriptnavi/properties/iimportparameterset-bulkdataloadingmode/">BulkDataLoadingMode</a>, <a href="../../../scriptnavi/properties/iimportparameterset-loadreturnmode/">LoadReturnMode</a>, <a href="../../../scriptnavi/properties/iimportparameterset-appendcheckgroupname/">AppendCheckGroupName</a>, <a href="../../../scriptnavi/objects/ipropertyhandling/">PropertyHandling</a>.<a href="../../../scriptnavi/properties/ipropertyhandling-autoupdatechncharacteristics/">AutoUpdateChnCharacteristics</a>, <a href="../../../scriptnavi/objects/ipropertyhandling/">PropertyHandling</a>.<a href="../../../scriptnavi/properties/ipropertyhandling-inheritanceseparator/">InheritanceSeparator</a>, <a href="../../../scriptnavi/objects/ipropertyhandling/">PropertyHandling</a>.<a href="../../../scriptnavi/properties/ipropertyhandling-inheritancemode/">InheritanceMode</a>, <a href="../../../scriptnavi/objects/ipropertyhandling/">PropertyHandling</a>.<a href="../../../scriptnavi/properties/ipropertyhandling-namingschema/">NamingSchema</a>, <a href="../../../scriptnavi/objects/ipropertyhandling/">PropertyHandling</a>.<a href="../../../scriptnavi/properties/ipropertyhandling-namemappingfile/">NameMappingFile</a>, and <a href="../../../scriptnavi/objects/ipropertyhandling/">PropertyHandling</a>.<a href="../../../scriptnavi/properties/ipropertyhandling-valuemappingfile/">ValueMappingFile</a>. The command ignores all other properties.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The page <a href="#" data-unresolved="1">Loading Bulk Data - General</a> contains important information on the extended loading behavior of TDM and TDMS files.<br attr="ext"/>The <a href="#" data-unresolved="1">Append Data</a> topic describes the behavior of DIAdem when you assign the value <span class="Monospace">Append</span> to the variable <span class="Monospace">ImportParameterSet</span> or when you assign the value <span class="Monospace">eAppend</span> to the <a href="../../../scriptnavi/objects/iimportparameterset/">ImportParameter</a> object of the <a href="../../../scriptnavi/properties/iimportparameterset-importmode/">ImportMode</a> property. If you want to append data from many files to channels in the Data Portal, you can improve speed by transferring the filenames as a composite text instead of calling the <span class="Monospace">DataFileLoadSel</span> command individually for each file. Separate the individual filenames in the composite text with the "|" character.</td></tr></table>
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
<tr><td width="150">FileImportFilter</td>
<td>Specifies which DataPlugin DIAdem uses for loading a data file into the Data Portal.<div id="exp_FileImportFilter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">If you do not specify a DataPlugin, DIAdem automatically uses the DataPlugin assigned to the file type.</p>
<p class="Body">The valid values for this variable vary according to the registered DataPlugin. The following values are valid:</p>
<table class="Borderless"><tr>
<td width="150"><strong>Value of the Variables</strong></td><td width="150"><strong>Meaning</strong></td>
<td><strong>Filename Extension</strong></td></tr><tr>
<td width="150"><span class="Monospace">TDM</span></td><td width="150">DIAdem TDM files</td>
<td><span class="Monospace">TDM</span></td></tr><tr>
<td width="150"><span class="Monospace">TDMS</span></td><td width="150">DIAdem TDM streaming files</td>
<td><span class="Monospace">TDMS</span></td></tr>
<tr><td width="150"><span class="Monospace">LVM</span></td><td width="150">LabVIEW LVM files</td>
<td><span class="Monospace">LVM</span></td></tr>
<tr><td width="150"><span class="Monospace">CSV</span></td><td width="150">Comma-separated values</td>
<td><span class="Monospace">CSV</span></td></tr>
<tr><td width="150"><span class="Monospace">DAT</span></td><td width="150">DIAdem DAT files</td>
<td><span class="Monospace">DAT</span></td></tr>
</table><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileImportFilter</span> variable for a file type, enable the <a href="#" data-unresolved="1">Recording mode</a> and open a file with the appropriate filename extension in the <a href="#" data-unresolved="1">Open</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../datafileload/">DataFileLoad</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Visit the <a href="#">DataPlugin Website</a> to find existing DataPlugins you can download.</td></tr></table>
</div></td></tr>
<tr><td width="150">ImportSelection</td>
<td>Specifies which data channels to load from a data file.<div id="exp_ImportSelection">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body"> If you do not assign a value to this variable, DIAdem loads all data channels. You can use the following syntax for the <span class="Monospace">ImportSelection</span> variable:</p>
<table class="Borderless"><tr><td width="30"><pre> <span class="Monospace">"[<em>GroupIndex</em>]/[<em>ChannelIndex</em>]"</span></pre></td><td>Uses indexes to specify which channels to load. The expression <span class="Monospace">"[1]/[2]"</span>, for example, loads the second channel of the first channel group. The expression <span class="Monospace">[2]/*</span> loads all channels from the second channel group. The expression <span class="Monospace">[2]/[2,5-8]</span> loads channel 2 and the channels 5 to 8 of the second channel group.</td></tr>
<tr><td width="30"><pre> <span class="Monospace"><em>"Identifier"</em></span></pre></td><td>Uses a condition to specify which channels to load. Use a question mark (?) as a wildcard for one character, and an asterisk (*) as a wildcard for any number of characters. The expression <span class="Monospace">"Example/D*"</span>, for example, specifies that DIAdem loads all channels with names starting with the letter <span class="Monospace">D</span> from the <span class="Monospace">Example</span> channel group. If the conditions do not meet the <a href="#" data-unresolved="1">name conventions</a> for channels, DIAdem replaces the invalid characters with valid characters.<br attr="ext"/>If you use the wildcard <span class="Monospace">*</span> for a channel group, DIAdem creates a new channel group in the Data Portal. If you enter channel numbers, DIAdem appends the selected channels to the default group in the Data Portal.</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  Use the vertical separator |, to load channels from several channel groups, for example, <span class="Monospace">Call DataFileLoadSel("Example.tdm","TDM","[1]/[2]|[2]/[4]|[3]/[5]","Load")</span>.</td></tr></table>
</div></td></tr>
<tr><td width="150">[ImportParameterSet]</td>
<td>Specifies how DIAdem imports data into the Data Portal. Use the <a href="../../../scriptnavi/objects/iimportparameterset/">ImportParameter</a> object for the <span class="Monospace">ImportParameterSet</span> parameter. You can also use one of the following script terms as an alternative. If the script term contains <span class="Monospace">"|ChnXYRelation"</span>, DIAdem maintains the reference to the x-channel for <a href="#" data-unresolved="1">xy-channels</a>.<div id="exp_ImportParameterSet">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless">
<tr>
<td><table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Load"</pre></donottranslate></td>
<td>Load</td></tr>
<tr><td width="150"><donottranslate><pre>"Load|ChnXYRelation"</pre></donottranslate></td>
<td>Load with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"Register"</pre></donottranslate></td>
<td>Register</td></tr>
<tr><td width="150"><donottranslate><pre>"Register|ChnXYRelation"</pre></donottranslate></td>
<td>Login with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"Append"</pre></donottranslate></td>
<td>Append</td></tr>
<tr><td width="150"><donottranslate><pre>"Append|ChnXYRelation"</pre></donottranslate></td>
<td>Append with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadImmediately"</pre></donottranslate></td>
<td>Always load bulk data</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadImmediately|ChnXYRelation"</pre></donottranslate></td>
<td>Always load bulk data with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnFirstAccess"</pre></donottranslate></td>
<td>Load bulk data on first access</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnFirstAccess|ChnXYRelation"</pre></donottranslate></td>
<td>Load bulk data with x-channel reference on first access</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnWriteAccess"</pre></donottranslate></td>
<td>Load bulk data when writing channel data</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnWriteAccess|ChnXYRelation"</pre></donottranslate></td>
<td>Load bulk data with x-channel reference when writing channel data</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td><a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a><br attr="ext"/>Element list with the elements. Use the <a href="../../../scriptnavi/properties/iimportparameterset-loadreturnmode/">LoadReturnMode</a> property to specify which elements the element list contains.</td></tr>
</table>
</div>

## Python example

```python
oMyElementList = dd.DataFileLoadSel("C:\\Example.tdm",None ,"[1]/[2,3]")
dd.ChnAverage(oMyElementList, "/Average")
```

```python
dd.DataFileLoadSel("C:\\Example.tdm","TDM","[1]/[2,3]","Register")
```

```python
dd.DataFileLoadSel(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm",None ,"[1]/[2]|[2]/[2]|[3]/[2]")
```

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")
oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingOnFirstAccess
oMyImportParameter.PropertyHandling.AutoUpdateChnCharacteristics = True
oMyImportParameter.PropertyHandling.InheritanceMode = dd.ePropInheritanceCopyToChannelLevel
dd.DataFileLoadSel("Example.tdm",None , "[1]/[2,3]", oMyImportParameter)
```

---

*Source: `ComOff/DataFileLoadSel.htm`*
