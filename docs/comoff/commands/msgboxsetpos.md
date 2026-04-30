---
title: "MsgBoxSetPos"
description: "Specifies the size and position of the next message box."
---

# MsgBoxSetPos

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MsgBoxSetPos

Specifies the size and position of the next message box.

## Signature

```python
dd.MsgBoxSetPos(MsgBoxXPos, MsgBoxYPos, MsgBoxWidth, MsgBoxHeight)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong>Use the <span class="Monospace">MsgBoxSetPos</span> command before the <a href="../msgboxdisp/">MsgBoxDisp</a> command that displays the message, because DIAdem deletes the set values and then displays messages with the default settings.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">MsgBoxXPos</td>
<td>Specifies the x-position of a message box in relation to the left edge.<div id="exp_MsgBoxXPos">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= MsgBoxXPos &lt;= 100</td></tr>
</table>
</div></td></tr>
<tr><td width="150">MsgBoxYPos</td>
<td>Specifies the y-position of a message box, in relation to the bottom edge.<div id="exp_MsgBoxYPos">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= MsgBoxYPos &lt;= 100</td></tr>
</table>
</div></td></tr>
<tr><td width="150">MsgBoxWidth</td>
<td>Specifies the width of a message box.<div id="exp_MsgBoxWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= MsgBoxWidth &lt;= 100</td></tr>
</table>
</div></td></tr>
<tr><td width="150">MsgBoxHeight</td>
<td>Specifies the height of a message box.<div id="exp_MsgBoxHeight">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= MsgBoxHeight &lt;= 100</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.MsgBoxSetPos(10, 10, 30, 20)
dd.MsgButtonTextSet("Step+1", "Step+2", "Step+3")
dd.MsgBoxDisp("Select next step","MB_YESNOCANCEL")
select_variable_0 = dd.MsgState
if (select_variable_0 == "IDYes") :
    dd.MsgBoxDisp("Step 1", "MB_OK", "MsgTypeNote",None , 5)
elif (select_variable_0 == "IDNo") :
    dd.MsgBoxDisp("Step 2", "MB_OK", "MsgTypeInformation",None , 5)
elif (select_variable_0 == "IDCancel") :
    dd.MsgBoxDisp("Step 3", "MB_OK", "MsgTypeWarning",None , 5)
dd.MsgNotModal = True
dd.MsgBoxDisp("Example completed", "MB_NOBUTTON", "MsgTypeNote",None , 10,dd.MsgNotModal)
```

---

*Source: `ComOff/MsgBoxSetPos.htm`*
