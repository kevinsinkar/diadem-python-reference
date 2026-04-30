---
title: "HdMarkAll"
description: "Marks all channel headers you want to save."
---

# HdMarkAll

!!! abstract "Command &middot; `ComOff.chm`"
    Command: HdMarkAll

Marks all channel headers you want to save.

## Signature

```python
dd.HdMarkAll()
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <span class="Monospace">HdMarkAll</span> command before the <a href="../hdsave/">HdSave</a> command so that DIAdem saves the channel header and the data set properties in the header file.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Python example

```python
dd.HdLoad("Test")
dd.FileChnName[1] = "NewName"
dd.HdMarkAll()
dd.HdSave("Test2")
```

---

*Source: `ComOff/HdMarkAll.htm`*
