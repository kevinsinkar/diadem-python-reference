---
title: "PkChNameSet"
description: "Renames a data channel displayed in the oscilloscope."
---

# PkChNameSet

!!! abstract "Command &middot; `PkVarOnl.chm`"
    Command: PkChNameSet

Renames a data channel displayed in the oscilloscope.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChannelNumber</td>
<td>Specifies the number of the data channel.<div id="exp_Channelnumber">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td class="monospace">1 ... Number of curves in the oscilloscope</td></tr>
</table>
</div></td></tr>
<tr><td width="150">Name</td>
<td>Specifies the channel name.<div id="exp_Name">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a>s</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
PkChNameSet(Channelnumber,Name)
```

---

*Source: `PkVarOnl/pkcomonl/PkChNameSet.htm`*
