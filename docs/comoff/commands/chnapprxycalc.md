---
title: "ChnApprXYCalc"
description: "Approximates a signal. DIAdem also generates the interpolation channel necessary for calculating the approximation."
---

# ChnApprXYCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnApprXYCalc

Approximates a signal. DIAdem also generates the interpolation channel necessary for calculating the approximation.

## Signature

```python
return_value = dd.ChnApprXYCalc( XW , Y , ResultChannel , ResultChannel , XChnStyle, XNo, XDiv)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You can select a maximum of ten setup functions simultaneously.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The values in the x-channel must be monotone increasing.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td style="width: 160px"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal. If the y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td style="width: 160px"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td style="width: 160px"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the interpolation points of the approximation function.</td></tr>
<tr><td style="width: 160px"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the approximation function.</td></tr>
<tr><td style="width: 160px">XChnStyle</td>
<td>Specifies which method DIAdem uses to generate the interpolation point channel.<div id="exp_XChnStyle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td><donottranslate><pre>"Partition complete area"</pre></donottranslate></td>
<td>Divide entire area</td></tr>
<tr><td><donottranslate><pre>"Partition intervals"</pre></donottranslate></td>
<td>Divide intervals</td></tr>
<tr><td><donottranslate><pre>"Use channel"</pre></donottranslate></td>
<td>Use channel</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td style="width: 160px">XNo</td>
<td>Specifies the number of values in a new data channel.<div id="exp_XNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>2 &lt;= XNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td style="width: 160px">XDiv</td>
<td>Specifies the number of equidistant sections in each interval of the x-range.<div id="exp_XDiv">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= XDiv &lt;= 100</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr>
<td style="width: 160px"><em>ChnResult</em></td>
<td>Contains two result channels. The first result channel contains the interpolation points and the second result channel contains the y-values of the approximation function. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
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
oMyResultChn = dd.ChnApprXYCalc(oMyXChannel, oMyYChannel, "Results/ApproximatedX", "Results/ApproximatedY", "Partition complete area", 100, 1)
print("Result channel(1): ", oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): ", oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Best Fit = " , oMyResultChn(2).Properties("Result~Approximation~ModelFunction").Value)
```

```python
dd.ApprAnsatzOff() # Deactivates all function terms
dd.ApprAnsatzFct[1] = "Yes" # Activates function term constant
dd.ApprAnsatzFct[2] = "Yes" # Activates function term x
dd.ApprAnsatzFct[3] = "Yes" # Activates function term x^2
oMyResultChn = dd.ChnApprXYCalc("[1]/[1]", "[1]/[2]", "Results/ApproximatedX", "Results/ApproximatedY", "Partition complete area", 100, 1)
print("1st Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"2nd Result channel: " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name  , "\r\n" ,"Best Fit = " , oMyResultChn(2).Properties("Result~Approximation~ModelFunction").Value)
```

---

*Source: `ComOff/ChnApprXYCalc.htm`*
