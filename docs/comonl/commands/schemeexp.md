---
title: "SchemeExp"
description: "Saves the currently open subblock diagram."
---

# SchemeExp

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: SchemeExp

Saves the currently open subblock diagram.

## Signature

```python
dd.SchemeExp(SchemeExpFile, SchemeOverwrite)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    SchemeExpFile = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SchemeExpFile</td>
<td>Specifies the subblock diagram file to be saved.<div id="exp_SchemeExpFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    SchemeExpFile = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div></td></tr>
<tr><td width="150">SchemeOverwrite</td>
<td>Specifies whether DIAdem overwrites a block diagram that has the same name as an existing block diagram, without a confirmation prompt.<div id="exp_SchemeOverwrite">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean Variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/SchemeExp.htm`*
