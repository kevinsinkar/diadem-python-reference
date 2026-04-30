---
title: "ChnApprYCalc"
description: "Approximates a signal."
---

# ChnApprYCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnApprYCalc

Approximates a signal.

## Signature

```python
return_value = dd.ChnApprYCalc( XW , Y , SamplingPointChn, ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You can select a maximum of ten setup functions simultaneously.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The values in the x-channel must be monotone increasing.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the selected setup function results in a curve that deviates substantially from the exact solution, DIAdem displays an error message.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <a href="../appransatzoff/">ApprAnsatzOff</a> command clears the checkboxes for the selected setup function terms.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal. If the y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td width="150">SamplingPointChn</td>
<td>Specifies the data channel containing the interpolation points.<div id="exp_SamplingPointChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the approximation function.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel containing the y-values of the approximation function. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.ApprAnsatzOff() # Deactivates all function terms
dd.ApprAnsatzFct[1] = "Yes" # Activates function term constant
dd.ApprAnsatzFct[2] = "Yes" # Activates function term x
dd.ApprAnsatzFct[3] = "Yes" # Activates function term x^2
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyY1Channel = dd.Data.Root.ChannelGroups(1).Channels(3)
oMyResultChn = dd.ChnApprYCalc(oMyXChannel, oMyYChannel, oMyY1Channel, "Results/ApproximatedY")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
dd.ApprAnsatzOff() # Deactivates all function terms
dd.ApprAnsatzFct[1] = "Yes" # Activates function term constant
dd.ApprAnsatzFct[2] = "Yes" # Activates function term x
dd.ApprAnsatzFct[3] = "Yes" # Activates function term x^2
oMyResultChn = dd.ChnApprYCalc("[1]/[1]","[1]/[2]","[1]/[3]","Results/ApproximatedY")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnApprYCalc.htm`*
