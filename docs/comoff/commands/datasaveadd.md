---
title: "DataSaveAdd"
description: "Saves data to an existing DIAdem DAT data file."
---

# DataSaveAdd

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataSaveAdd

Saves data to an existing DIAdem DAT data file.

## Signature

```python
dd.DataSaveAdd(DataFile, ChnList, [DataFileCode])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DataFile</td>
<td>Specifies the name of the current data file.<div id="exp_DataFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">[DataFileCode]</td>
<td>Specifies the coding procedure for DAT data files. By default DIAdem saves the data file in <span class="Monospace">Unicode</span>.<div id="exp_DataFileCode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Ansi"</pre></donottranslate></td>
<td>ANSI</td></tr>
<tr><td width="150"><donottranslate><pre>"Unicode"</pre></donottranslate></td>
<td>Unicode</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[1]/Channel*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
dd.DataSaveAdd(dd.DataWritePath + "MyExample1.dat", oMyChannelList)
```

---

*Source: `ComOff/DataSaveAdd.htm`*
