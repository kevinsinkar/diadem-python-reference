---
title: "SchemeSave"
description: "Saves the current block diagram under a new name."
---

# SchemeSave

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: SchemeSave

Saves the current block diagram under a new name.

## Signature

```python
dd.SchemeSave(SchemeFile, [SchemeOverwrite])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The command <span class="Monospace">SchemeSave</span> saves block diagrams on the <a href="../../../varonl/variables/dacwritepath/">DAC User Path</a>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SchemeFile</td>
<td>Specifies the name of the current block diagram.<div id="exp_SchemeFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[SchemeOverwrite]</td>
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

*Source: `ComOnl/SchemeSave.htm`*
