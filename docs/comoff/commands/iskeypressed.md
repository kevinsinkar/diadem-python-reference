---
title: "IsKeyPressed"
description: "Specifies whether the specified key was pressed."
---

# IsKeyPressed

!!! abstract "Command &middot; `ComOff.chm`"
    Command: IsKeyPressed

Specifies whether the specified key was pressed.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">KeyValue</td>
<td>Specifies the pressed key.<div id="exp_KeyValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>-2147483648 &lt;= KeyValue &lt;= 2147483647</td></tr>
</table>The following list contains some possible values. You can find a detailed list on the internet under the search term "Virtual Keys". The Hex value and the associated key are specified.<br attr="ext"/><table class="Borderless"><tr><td width="150">&amp;H01</td><td>Left mouse button</td></tr><tr><td width="150">&amp;H02</td><td>Right mouse button</td></tr><tr><td width="150">&amp;H04</td><td>Middle mouse button</td></tr><tr><td width="150">&amp;H10</td><td>&lt;Shift&gt; key</td></tr><tr><td width="150">&amp;H11</td><td>CTRL key</td></tr><tr><td width="150">&amp;H1B</td><td>ESC key</td></tr><tr><td width="150">&amp;H20</td><td>Spacebar</td></tr><tr><td width="150">&amp;H0D</td><td>Enter key</td></tr><tr><td width="150">&amp;H70 to &amp;H87H</td><td>F1- to F24 keys</td></tr><tr><td width="150">&amp;H41 to &amp;H5A</td><td>A- to Z keys</td></tr><tr><td width="150">&amp;H30 to &amp;H39</td><td>0- to 9 keys</td></tr><tr><td width="150">&amp;H60 to &amp;H69</td><td>0- to 9 keys on the numeric block</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type.</td></tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp("Press space bar.",None ,None ,None ,5,True)
while (not dd.IsKeyPressed(0x20)):
    dd.KeyWait()
dd.MsgBoxDisp("Space bar pressed")
```

---

*Source: `ComOff/IsKeyPressed.htm`*
