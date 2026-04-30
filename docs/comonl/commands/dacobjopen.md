---
title: "DACObjOpen"
description: "Opens a DAC object to set the parameters for the object."
---

# DACObjOpen

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DACObjOpen

Opens a DAC object to set the parameters for the object.

## Signature

```python
dd.DACObjOpen(DacObjName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    DACObjName = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>DAC objects are usually DAC blocks but also can be sub-block diagrams, terminals, or dialog boxes.</td></tr></table>
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

---

*Source: `ComOnl/DACObjOpen.htm`*
