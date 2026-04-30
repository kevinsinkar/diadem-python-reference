---
title: "DACObjWhere"
description: "Searches for DAC blocks in the current block diagram."
---

# DACObjWhere

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DACObjWhere

Searches for DAC blocks in the current block diagram.

## Signature

```python
dd.DACObjWhere(DacObjName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    DACObjName = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>DAC objects are usually DAC blocks but also can be sub-block diagrams, terminals, or dialog boxes.</td></tr></table>
<table class="Borderless" id="table3"><tr><td class="Icon"><img height="25" src="./image/note.gif" width="26"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    DACObjName = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre></donottranslate>
</td></tr></table>
<table class="Borderless" id="table4"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If DIAdem finds the DAC block in a subblock diagram, DIAdem opens this subblock diagram. If DIAdem does not find the DAC block in the current block diagram, the return parameter <span class="Monospace">DACObjName</span> contains an empty string.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DacObjName</td>
<td>Specifies the name of a DAC object.<div id="exp_DacObjName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 16 characters</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    DACObjName = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>DAC objects are usually DAC blocks but also can be sub-block diagrams, terminals, or dialog boxes.</td></tr></table>
<p>
</p></div></td></tr>
</table>
</div>

## Python example

```python
dd.DACObjWhere("MyBlock")
if dd.DacObjName!="" :
    dd.DacObjOpen(dd.DacObjName + "._Scheme_")
else:
    print("Block not found.")
```

---

*Source: `ComOnl/DACObjWhere.htm`*
