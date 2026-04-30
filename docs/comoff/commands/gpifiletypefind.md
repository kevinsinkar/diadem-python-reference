---
title: "GPIFileTypeFind"
description: "Specifies the name of a GPI file filter."
---

# GPIFileTypeFind

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GPIFileTypeFind

Specifies the name of a GPI file filter.

## Signature

```python
dd.GPIFileTypeFind(FileDlgFilt)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileDlgFilt</td>
<td>Specifies the file type.<div id="exp_FileDlgFilt">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>The variable <span class="Monospace">FileDlgFilt</span> contains the description and the file filter separated by a comma, for example <span class="Monospace">“Script Files,*.VBS”</span> or <span class="Monospace">“Excel Files, *.csv;*.xls”</span>. You can also specify several file types separated by a vertical line, for example <span class="Monospace">“Script Files,*.VBS|List Files,*.LST”</span>.</p>
<p>In the command <span class="Monospace">FileNameGet</span>, you can only use the variable <span class="Monospace">FileDlgFilt</span> if you assign the value <span class="Monospace">ANY</span> or <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable. If you assign the value <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable, DIAdem interprets the variable <span class="Monospace">FileDlgFilt</span> as the name of the associated DataPlugin.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/GPIFileTypeFind.htm`*
