---
title: "HdSave"
description: "Saves a data set header file in the DAT format."
---

# HdSave

!!! abstract "Command &middot; `ComOff.chm`"
    Command: HdSave

Saves a data set header file in the DAT format.

## Signature

```python
dd.HdSave(HdFile)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">HdFile</td>
<td>Specifies the name of a data set header file in the DAT format.<div id="exp_HdFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
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

*Source: `ComOff/HdSave.htm`*
