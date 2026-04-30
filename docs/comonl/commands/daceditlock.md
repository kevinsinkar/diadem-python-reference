---
title: "DACEditLock"
description: "Locks the configuration of a block diagram or unlocks it."
---

# DACEditLock

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DACEditLock

Locks the configuration of a block diagram or unlocks it.

## Signature

```python
dd.DACEditLock(DACEditLockState)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DACEditLockState</td>
<td>Determines whether the configuration of a block diagram is locked.<div id="exp_DACEditLockState">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
if dd.DACEditLockState :
    dd.DACEditLock(False)
```

---

*Source: `ComOnl/DACEditLock.htm`*
