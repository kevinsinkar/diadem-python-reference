---
title: "HdCopy"
description: "Copies a channel header from one channel to another channel."
---

# HdCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: HdCopy

Copies a channel header from one channel to another channel.

## Signature

```python
dd.HdCopy(HdChnArg1, HdChnArg2)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">HdChnArg1</td>
<td>Uses the channel name or the channel number to specify a channel.<div id="exp_HdChnArg1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word</a></td></tr>
<tr>
<td>1 &lt;= HdChnArg1 &lt;= <a href="../../../varoff/variables/actfilehdno/">ActFileHdNo</a><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">HdChnArg2</td>
<td>Uses the channel name or the channel number to specify a target channel.<div id="exp_HdChnArg2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word</a></td></tr>
<tr>
<td>1 &lt;= HdChnArg1 &lt;= <a href="../../../varoff/variables/actfilehdno/">ActFileHdNo</a><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.GHdChnNo = 1
dd.GHdChnLength = 20
dd.GHdChnType = "EXPLICIT"
dd.GHdDispFormat= "Numeric"
dd.GHdChnFile = "Test.asc"
dd.GHdSaveType = "CHANNEL"
dd.GHdChnIdx = 4
dd.GHdChnMode = "ASCII"
dd.GHdAsciiPtr = 1
dd.GHdDecChar = "."
dd.GHdExChar = "E"
dd.GHdSep = ","
dd.GHdOffs = 0
dd.HdCreate()
dd.HdCopy("[1]/[1]","[1]/[2]")
dd.FileChnStep[2]= 5
dd.FileChnBeginVal[2]= 50
dd.HdMarkAll()
dd.HdSave("Test")
```

---

*Source: `ComOff/HdCopy.htm`*
