---
title: "FontPointsToPixels"
description: "Converts a font size into pixel. DIAdem includes the DPI settings of the system."
---

# FontPointsToPixels

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FontPointsToPixels

Converts a font size into pixel. DIAdem includes the DPI settings of the system.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FontPoints</td>
<td>Specifies the font size in points.<div id="exp_FontPoints">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= FontPoints &lt;= 1E300</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is an <a href="#" data-unresolved="1">Integer variable</a> type.</td></tr>
</table>
</div>

## Python example

```python
Control.Font = -dd.FontPointsToPixels(8) + ",0,0,0,700,0,0,0,0,3,2,1,34,Arial"
```

---

*Source: `ComOff/FontPointsToPixels.htm`*
