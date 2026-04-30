---
title: "MsgButtonTextSet"
description: "Changes the button labels in the next message box."
---

# MsgButtonTextSet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MsgButtonTextSet

Changes the button labels in the next message box.

## Signature

```python
dd.MsgButtonTextSet([MsgButtonText1], [MsgButtonText2], [MsgButtonText3])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <span class="Monospace">MsgButtonTextSet</span> command before the <a href="../msgboxdisp/">MsgBoxDisp</a> command that displays the message, because DIAdem deletes the set values and then displays messages with the default settings.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[MsgButtonText1]</td>
<td>Specifies the label text for the first button in a message box. By default the <span class="Monospace">MsgButtonType</span> parameter of the subsequent command <span class="Monospace">MsgBoxDisp</span> specifies the button labels.<div id="exp_MsgButtonText1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[MsgButtonText2]</td>
<td>Specifies the label text for the second button in a message box. By default the <span class="Monospace">MsgButtonType</span> parameter of the subsequent command <span class="Monospace">MsgBoxDisp</span> specifies the button labels.<div id="exp_MsgButtonText2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[MsgButtonText3]</td>
<td>Specifies the label text for the third button in a message box. By default the <span class="Monospace">MsgButtonType</span> parameter of the subsequent command <span class="Monospace">MsgBoxDisp</span> specifies the button labels.<div id="exp_MsgButtonText3">
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

*Source: `ComOff/MsgButtonTextSet.htm`*
