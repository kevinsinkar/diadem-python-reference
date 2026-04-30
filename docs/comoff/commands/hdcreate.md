---
title: "HdCreate"
description: "Generates external channel headers."
---

# HdCreate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: HdCreate

Generates external channel headers.

## Signature

```python
dd.HdCreate()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Python example

```python
dd.HdDelAll()
dd.GHdChnNo = 4
dd.GHdChnLength = 6
dd.GHdChnType = "EXPLICIT"
dd.GHdDispFormat= "Numeric"
dd.GHdChnFile = "MyFile.asc"
dd.GHdSaveType = "CHANNEL"
dd.GHdChnIdx = 4
dd.GHdChnMode = "ASCII"
dd.GHdAsciiPtr = 1
dd.GHdDecChar = "."
dd.GHdExChar = "E"
dd.GHdSep = ","
dd.GHdOffs = 0
dd.HdCreate()
dd.HdMarkAll()
dd.HdSave("MyFile")
```

---

*Source: `ComOff/HdCreate.htm`*
