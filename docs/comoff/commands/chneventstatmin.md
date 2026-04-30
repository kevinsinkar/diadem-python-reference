---
title: "ChnEventStatMin"
description: "Specifies the minimum value of an individual event or of all events from the result list of an event search."
---

# ChnEventStatMin

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventStatMin

Specifies the minimum value of an individual event or of all events from the result list of an event search.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnArg1</td>
<td>Specifies a channel.<div id="exp_ChnArg1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to clearly specify channels.</p>
</div></td></tr>
<tr><td width="150">ChnEventList</td>
<td>Contains the search result or the result of a logical operation from several searches.<div id="exp_ChnEventList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">This variable corresponds to a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">[ChnEventListIndex]</td>
<td>Specifies the index of the event. If the index is not specified or if <span class="Monospace">Null</span> is specified, DIAdem includes all events.<div id="exp_ChnEventListIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventResultValueType]</td>
<td>Specifies whether DIAdem returns the value or the index of the wanted value. By default, DIAdem returns the value.<div id="exp_ChnEventResultValueType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Value"</pre></donottranslate></td>
<td>Value</td></tr>
<tr><td width="150"><donottranslate><pre>"Index"</pre></donottranslate></td>
<td>Index</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Floating-point number</a> type.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
sOutPut = "Statistic results for events:" + "\r\n" + "Minimum: "
for iCount in range( 1, dd.ChnEventCount(dd.ChnEventResultList)+1):
    sOutPut = sOutPut + " Event " + iCount + ": " + dd.Str(dd.ChnEventStatMin("[1]/[2]", dd.ChnEventResultList, iCount),"ENGd.ddd")
print(sOutPut)
```

---

*Source: `ComOff/ChnEventStatMin.htm`*
