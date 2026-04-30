---
title: "VEnumIdx"
description: "Specifies the index of a selection term from an enumeration variable or from a dynamic enumeration variable ."
---

# VEnumIdx

!!! abstract "Command &middot; `ComOff.chm`"
    Command: VEnumIdx

Specifies the index of a selection term from an enumeration variable or from a dynamic enumeration variable .

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ItemName</td>
<td>Specifies the name of a DIAdem variable or of a DIAdem command.<div id="exp_ItemName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ItemValue</td>
<td>Specifies the selection term.<div id="exp_ItemValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 255 characters</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is an <a href="#" data-unresolved="1">Integer variable</a> type. Receives the index of the selection term. Counting starts from <span class="Monospace">1</span>. The return value is <span class="Monospace">-1</span> if DIAdem does not find the selection term</td></tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp (dd.VEnumIdx("WndMode","MAXIMIZE"))
```

---

*Source: `ComOff/VEnumIdx.htm`*
