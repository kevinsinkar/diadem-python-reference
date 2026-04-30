---
title: "ColorChoose"
description: "Opens the dialog box for color selection."
---

# ColorChoose

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ColorChoose

Opens the dialog box for color selection.

## Signature

```python
dd.ColorChoose(FileDlgCaption, ChoosedColor)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not assign a value to the <span class="Monospace">FileDlgCaption</span> variable, DIAdem generates the caption automatically.</td>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="#" data-unresolved="1">RGB function</a> to calculate the RGB color value from the individual colors.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileDlgCaption</td>
<td>Specifies the dialog box caption.<div id="exp_FileDlgCaption">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not assign a value to the <span class="Monospace">FileDlgCaption</span> variable, DIAdem generates the caption automatically.</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChoosedColor</td>
<td>Specifies the RGB color value.<div id="exp_ChoosedColor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="#" data-unresolved="1">RGB function</a> to calculate the RGB color value from the individual colors.</td></tr></table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.ChoosedColor = 255
dd.ColorChoose ("Choose Color", dd.ChoosedColor)
dd.MsgBoxDisp ("Selected color: " + dd.ChoosedColor)
```

---

*Source: `ComOff/ColorChoose.htm`*
