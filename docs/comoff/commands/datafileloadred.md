---
title: "DataFileLoadRed"
description: "Loads data files into the DIAdem Data Portal and simultaneously reduces the data."
---

# DataFileLoadRed

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileLoadRed

Loads data files into the DIAdem Data Portal and simultaneously reduces the data.

## Signature

```python
return_value = dd.DataFileLoadRed(DataFilename, FileImportFilter, ImportSelection, IntervalMethod, IntervalValue, ReductionType, [SectionBegin], [SectionEnd], [ ChnXYRelation ])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileImportFilter</span> variable for a file type, enable the <a href="#" data-unresolved="1">Recording mode</a> and open a file with the appropriate filename extension in the <a href="#" data-unresolved="1">Open</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../datafileload/">DataFileLoad</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Visit the <a href="#">DataPlugin Website</a> to find existing DataPlugins you can download.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  Use the vertical separator |, to load channels from several channel groups, for example, <span class="Monospace">Call DataFileLoadSel("Example.tdm","TDM","[1]/[2]|[2]/[4]|[3]/[5]","Load")</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">ReductionType</span> variable can accept one of the values that result from the bitwise comparison (<a href="#" data-unresolved="1">Or-Operator</a>) of the followiing constant values: <a href="../../../varoff/variables/einterfirstvalue/">eInterFirstValue</a> (1), <a href="../../../varoff/variables/einterminimum/">eInterMinimum</a> (2), <a href="../../../varoff/variables/eintermaximum/">eInterMaximum</a> (4), <a href="../../../varoff/variables/eintermeanvalue/">eInterMeanValue</a> (8)</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem creates a new data channel for each reduction method. To do this, DIAdem appends the following text to the original channel name:<table class="Borderless"><tr><td width="150"><strong>Reduction method</strong></td><td width="150"><strong>Constant</strong></td><td><strong>Channel name suffix</strong></td></tr><tr><td width="150">1. Value</td><td width="150"><a href="../../../varoff/variables/einterfirstvalue/">eInterFirstValue</a> (1)</td><td>_Sample</td></tr><tr><td width="150">Minimum</td><td width="150"><a href="../../../varoff/variables/einterminimum/">eInterMinimum</a> (2)</td><td>_Min</td></tr><tr><td width="150">Maximum</td><td width="150"><a href="../../../varoff/variables/eintermaximum/">eInterMaximum</a> (4)</td><td>_Max</td></tr><tr><td width="150">Arithmetic mean</td><td width="150"><a href="../../../varoff/variables/eintermeanvalue/">eInterMeanValue</a> (8)</td><td>_Mean</td></tr></table>
</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the two variables <a href="../../../varoff/variables/sectionbegin/">SectionBegin</a> and <a href="../../../varoff/variables/sectionend/">SectionEnd</a> both have the value 0 or are not transferred, DIAdem loads the complete channel. The interval from <span class="Monospace">SectionBegin</span> to <span class="Monospace">SectionEnd</span> must not be larger than the value of the <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a> variable.<br attr="ext"/>To load a data section without reducing data in any way, select the value <span class="Monospace">"IntervalWidth",</span> for the <a href="../../../varoff/variables/intervalmethod/">IntervalMethod</a> variable, select the value <span class="Monospace">1</span> as the <a href="../../../varoff/variables/intervalvalue/">IntervalValue</a> interval width, and select the value <span class="Monospace">eInterFirstValue</span> as the <a href="../../../varoff/variables/reductiontype/">ReductionType</a> reduction type.</td></tr></table>
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
<td>Specifies the DataPlugin DIAdem uses for loading a data file into the Data Portal.<div id="exp_FileImportFilter">
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
<tr><td width="150">IntervalMethod</td>
<td>Specifies whether DIAdem divides a channel into a specific number of intervals or whether you enter the number of values per interval.<div id="exp_IntervalMethod">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"IntervalCount"</pre></donottranslate></td>
<td>No. of intervals</td></tr>
<tr><td width="150"><donottranslate><pre>"IntervalWidth"</pre></donottranslate></td>
<td>Interval width</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">IntervalValue</td>
<td>Specifies the number of intervals or the interval width, depending on which value <span class="Monospace">IntervalMethod</span> contains.<div id="exp_IntervalValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= IntervalValue &lt;= 2147483646</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ReductionType</td>
<td>Specifies the data reduction method. You can select several reduction methods simultaneously. DIAdem creates a new data channel for each reduction method.<div id="exp_ReductionType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>1 &lt;= ReductionType &lt;= 15</td></tr>
</table>
<p>DIAdem moves a window over the data channel step-by-step, and loads values from each interval, according to the selected loader: 1. value, minimum, maximum, or arithmetic mean.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">ReductionType</span> variable can accept one of the values that result from the bitwise comparison (<a href="#" data-unresolved="1">Or-Operator</a>) of the followiing constant values: <a href="../../../varoff/variables/einterfirstvalue/">eInterFirstValue</a> (1), <a href="../../../varoff/variables/einterminimum/">eInterMinimum</a> (2), <a href="../../../varoff/variables/eintermaximum/">eInterMaximum</a> (4), <a href="../../../varoff/variables/eintermeanvalue/">eInterMeanValue</a> (8)</td></tr></table><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem creates a new data channel for each reduction method. To do this, DIAdem appends the following text to the original channel name:<table class="Borderless"><tr><td width="150"><strong>Reduction method</strong></td><td width="150"><strong>Constant</strong></td><td><strong>Channel name suffix</strong></td></tr><tr><td width="150">1. Value</td><td width="150"><a href="../../../varoff/variables/einterfirstvalue/">eInterFirstValue</a> (1)</td><td>_Sample</td></tr><tr><td width="150">Minimum</td><td width="150"><a href="../../../varoff/variables/einterminimum/">eInterMinimum</a> (2)</td><td>_Min</td></tr><tr><td width="150">Maximum</td><td width="150"><a href="../../../varoff/variables/eintermaximum/">eInterMaximum</a> (4)</td><td>_Max</td></tr><tr><td width="150">Arithmetic mean</td><td width="150"><a href="../../../varoff/variables/eintermeanvalue/">eInterMeanValue</a> (8)</td><td>_Mean</td></tr></table>
</td></tr></table>
</div></td></tr>
<tr><td width="150">[SectionBegin]</td>
<td>Specifies the first channel line index of the channel section that DIAdem loads.<div id="exp_SectionBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p>Value range: 0 &lt;= SectionBegin &lt;= (2^52)-1</p>
</div></td></tr>
<tr><td width="150">[SectionEnd]</td>
<td>Specifies the last channel line index of the channel section that DIAdem loads.<div id="exp_SectionEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p>Value range: 0 &lt;= SectionEnd &lt;= (2^52)-1</p>
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

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="../../../inavidata/collections/elementlist/">ElementList object</a> type. The ElementList contains all data elements created in the Data Portal by the command. A superordinate element describes its subordinate element if the superordinate element was created. If the Data Portal is empty during the loading process, DIAdem returns the Root element. If DIAdem creates a channel group containing several channels, the channel group is returned. If DIAdem loads a channel into the default group, the channel is returned.</td></tr>
</table>
</div>

## Python example

```python
oMyElementList = dd.DataFileLoadRed("Example.tdm","TDM","","IntervalWidth",100,dd.eInterMeanValue or dd.eInterFirstValue)
dd.ChnAverage(oMyChannelList, "/Average")
```

---

*Source: `ComOff/DataFileLoadRed.htm`*
