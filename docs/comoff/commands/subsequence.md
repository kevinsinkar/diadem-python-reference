---
title: "SubSequence"
description: "Identifies a subscript."
---

# SubSequence

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SubSequence

Identifies a subscript.

## Signature

```python
dd.SubSequence([SubSequenceText])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[SubSequenceText]</td>
<td>Specifies text for a note that comments a subscript. By default the <span class="Monospace">SubSequenceText</span> variable contains an empty text.<div id="exp_SubSequenceText">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
# Register all functions and procedures of Function_Library.vbs
ScriptInclude("Function_Library")
# Calling the function envelope curve
GetChnName(1)
MsgBoxDisp (strChannelName)
GetChnName(5)
MsgBoxDisp (strChannelName)
```

```python
# Labelling as subscript
Subsequence()
# Initialization
# Procedure for evaluating a channel name
def GetChnName(intChannelId):
    strChannelName ="" ' Initialize string
    if intChannelNo <= dd.Data.Root.ActiveChannelGroup.Channels.Count:
        ' Less then maximum channel number
    strChannelName = dd.Data.Root.ActiveChannelGroup.Channels(intChannelId)
```

---

*Source: `ComOff/SubSequence.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
