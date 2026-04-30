---
title: "Signif"
description: "Rounds the value of the first parameter mathematically to the number of significant places specified in the second parameter."
---

# Signif

!!! abstract "Command &middot; `ComOff.chm`"
    Command: Signif

Rounds the value of the first parameter mathematically to the number of significant places specified in the second parameter.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">Value</td>
<td>Specifies the value to round.<div id="exp_Value">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">Value</td>
<td>Specifies the number of significant places.<div id="exp_Value__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Floating-point number</a> type.</td></tr>
</table>
</div>

## Python example

```python
Result = dd.Signif(22499, 2) # =>  22000
Result = dd.Signif(22501, 2) # =>  23000
Result = dd.Signif(22500, 2) # =>  22000
Result = dd.Signif(23500, 2) # =>  23000
Result = dd.Signif(23.499, 2) # =>  23
Result = dd.Signif(23.499, 3) # =>  23.5
Result = dd.Signif(23.449, 4) # =>  23.45
```

---

*Source: `ComOff/Signif.htm`*
