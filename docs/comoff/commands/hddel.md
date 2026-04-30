---
title: "HdDel"
description: "Deletes an external channel header."
---

# HdDel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: HdDel

Deletes an external channel header.

## Signature

```python
dd.HdDel(HdChnArg1)
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
</table>
</div>

## Python example

```python
dd.HdLoad("Test")
dd.HdDel("[1]/[3]")
dd.DataFileLoad("Drive.dat","DAT")
```

---

*Source: `ComOff/HdDel.htm`*
