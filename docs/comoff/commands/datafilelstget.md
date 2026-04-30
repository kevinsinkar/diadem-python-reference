---
title: "DataFileLstGet"
description: "Reads a DIAdem file that is a .tdm , .tdms , or .dat type, and creates a list of the associated binary files. The list does not contain video files if the data "
---

# DataFileLstGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileLstGet

Reads a DIAdem file that is a .tdm , .tdms , or .dat type, and creates a list of the associated binary files. The list does not contain video files if the data file contains video channels.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The first element in the vector variable <span class="Monospace">DataFileLst</span> contains the name of the Dat header file.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FSSourceName</td>
<td>Specifies the source file or source folder for DIAdem file and folder commands.<div id="exp_FSSourceName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum <a href="../../../varoff/variables/applicationmaxpathlength/">ApplicationMaxPathLength</a> characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
</div></td></tr>
<tr><td width="150">[DataFileLstMode]</td>
<td>Specifies whether you store the names of the selected files with absolute paths or without paths.<div id="exp_DataFileLstMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr>
<td>0 &lt;= DataFileLstMode &lt;= 65535<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>If you assign the value 1 to the <span class="Monospace">DataFileLstMode</span> variable, you save the names without a path. If you assign the value 2 to the <span class="Monospace">DataFileLstMode</span> variable, you save the names with a path. The default value of the variable is 1.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the number of files found. The return value is a DataFileLstLen type.<div id="exp_DataFileLstLen">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr>
<td>0 &lt;= DataFileLstLen &lt;= 65535<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
if dd.FileExist(dd.DataReadPath + "Drive.dat") :
    for intCount in range( 1, dd.DataFileLstGet(dd.DataReadPath + "Drive")+1):
        dd.MsgBoxDisp(dd.DataFileLst(intCount))
```

---

*Source: `ComOff/DataFileLstGet.htm`*
