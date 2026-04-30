---
title: "RGB"
description: "Specifies the RGB color value."
---

# RGB

!!! abstract "Command &middot; `ComOff.chm`"
    Command: RGB

Specifies the RGB color value.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">RedValue</td>
<td>Specifies the proportion of red in the color.<div id="exp_RedValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word</a></td></tr>
<tr>
<td>0 &lt;= RedValue &lt;= 255<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GreenValue</td>
<td>Specifies the proportion of green in the color.<div id="exp_GreenValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word</a></td></tr>
<tr>
<td>0 &lt;= GreenValue &lt;= 255<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">BlueValue</td>
<td>Specifies the proportion of blue in the color.<div id="exp_BlueValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word</a></td></tr>
<tr>
<td>0 &lt;= BlueValue &lt;= 255<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the RGB color value. The return value is a <a href="#" data-unresolved="1">Integer</a> type.</td></tr>
</table>
</div>

## Python example

```python
dd.Report.Settings.Page.BackgroundColor.ColorIndex =dd.eColorIndexOtherColors
dd.Report.Settings.Page.BackgroundColor.RGB = dd.RGB(0,255,0) # Green
dd.Report.Refresh()
```

---

*Source: `ComOff/RGB.htm`*
