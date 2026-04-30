---
title: "DACObjDlg"
description: "Specifies the dialog box title of a DAC block."
---

# DACObjDlg

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DACObjDlg

Specifies the dialog box title of a DAC block.

## Signature

```python
dd.DACObjDlg(BlDlg)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    <em>Value</em> = BlDlg
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">BlDlg</span> variable is read-only.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="./image/note.gif" width="26"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<pre><donottranslate>
Call DACObjOpen(BlockName)
      Value = BlDlg
Call DACObjClose(BlockName)</donottranslate></pre>
<p>
<br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</p></td></tr></table>
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call DACObjDlg(<em>DialogName</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">BlDlg</td>
<td>Specifies the dialog box title of an open DAC block.<div id="exp_BlDlg">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    <em>Value</em> = BlDlg
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">BlDlg</span> variable is read-only.</td></tr></table>
<p>
</p></div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">BlDlg</td>
<td>Receives the dialog box title of the open block if the <span class="Monospace">BlDlg</span> variable transfers an empty text as the input parameter.<div id="exp_BlDlg01">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="./image/note.gif" width="26"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<pre><donottranslate>
Call DACObjOpen(BlockName)
      Value = BlDlg
Call DACObjClose(BlockName)</donottranslate></pre>
<p>
<br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</p></td></tr></table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.DacObjOpen("Input01")
dd.DacObjDlg("")
dd.SUDDlgShow(dd.BlDlg,dd.ResourceDrv + dd.BlDlg)
dd.DacObjClose(dd.BlActName)
```

---

*Source: `ComOnl/DACObjDlg.htm`*
