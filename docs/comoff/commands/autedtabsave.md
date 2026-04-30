---
title: "AutEdTabSave"
description: "Saves a file that is open in the script editor."
---

# AutEdTabSave

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdTabSave

Saves a file that is open in the script editor.

## Signature

```python
dd.AutEdTabSave(AutEdTabIndex, [AutEdTabName])
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
<tr><td width="150">[AutEdTabName]</td>
<td>Specifies the name you use to save a file in the script editor. By default the <span class="Monospace">AutEdTabName</span> variable contains the name of the loaded file.<div id="exp_AutEdTabName">
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
dd.AutEdInfoGet()
dd.FileDlgName = dd.AutEdName
dd.AutEdSaveAsDlg(dd.FileDlgName)
intLoop = 0
if dd.DlgState == "IDOk" :
    dd.AutEdTabNameGet(intLoop)
    while (intLoop < dd.AutEdNoFiles and dd.AutEdTabName != dd.AutEdName):
        intLoop = intLoop +1
        dd.AutEdTabNameGet(intLoop)
    dd.AutEdTabSave(intLoop,dd.FileDlgName)
```

---

*Source: `ComOff/AutEdTabSave.htm`*
