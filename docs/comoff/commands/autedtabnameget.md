---
title: "AutEdTabNameGet"
description: "Returns the name of a file that is loaded in the script editor."
---

# AutEdTabNameGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdTabNameGet

Returns the name of a file that is loaded in the script editor.

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

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the name of the file in the script editor. The return value is a AutEdTabName type.<div id="exp_AutEdTabName">
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
strMsg = "List of open files: " + "\r\n"
for intLoop in range( 0, dd.AutEdNoFiles -1+1):
    MyAutEdTabName = dd.AutEdTabNameGet(intLoop)
    strMsg = strMsg + MyAutEdTabName + "\r\n"
dd.MsgBoxDisp(strMsg)
```

---

*Source: `ComOff/AutEdTabNameGet.htm`*
