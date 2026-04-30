---
title: "AutEdTabActivate"
description: "Enables a file that is open in the script editor."
---

# AutEdTabActivate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdTabActivate

Enables a file that is open in the script editor.

## Signature

```python
dd.AutEdTabActivate(AutEdTabIndex)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">AutEdTabIndex</td>
<td>Specifies the index of a file that is open in the script editor.<div id="exp_AutEdTabIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">The index count starts with zero.</p>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.AutEdInfoGet()
for intLoop in range( 0, dd.AutEdNoFiles-1+1):
    dd.AutEdTabActivate (intLoop)
    dd.Pause (1)
```

---

*Source: `ComOff/AutEdTabActivate.htm`*
