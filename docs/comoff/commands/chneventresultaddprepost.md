---
title: "ChnEventResultAddPrePost"
description: "Adds a number of values or a value range at the beginning or the end of a search result. The index of advanced search results is never smaller than one or great"
---

# ChnEventResultAddPrePost

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventResultAddPrePost

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('ChnEventResultList', ...)   # instead of dd.ChnEventResultList = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Adds a number of values or a value range at the beginning or the end of a search result. The index of advanced search results is never smaller than one or greater than the channel length of the input channel. If the extended areas of the search results overlap, the command combines these areas to one area.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnEventList</td>
<td>Contains the search result or the result of a logical operation from several searches.<div id="exp_ChnEventList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">This variable corresponds to a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">SourceChn</td>
<td>Specifies the input channel.<div id="exp_SourceChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to specify channels.</p>
</div></td></tr>
<tr><td width="150">ChnEventResultAddPreValue</td>
<td>Specifies the number of values or the value range by which DIAdem extends the result of an event backwards.<div id="exp_ChnEventResultAddPreValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>-2147483647 &lt;= ChnEventResultAddPreValue &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventResultAddPostValue</td>
<td>Specifies the number of values or the value range by which DIAdem extends the result of an event forward.<div id="exp_ChnEventResultAddPostValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>-2147483647 &lt;= ChnEventResultAddPostValue &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventValueType</td>
<td>Specifies whether DIAdem adds the number of values of the input channel or the value range of the input channel to the search results.<div id="exp_ChnEventValueType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Index"</pre></donottranslate></td>
<td>Number of values</td></tr>
<tr><td width="150"><donottranslate><pre>"Value"</pre></donottranslate></td>
<td>Value range</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventListIndex]</td>
<td>Specifies the index of the event. If the index is not specified or if <span class="Monospace">Null</span> is specified, DIAdem includes all events.<div id="exp_ChnEventListIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>A return value is a two-dimensional array containing the extended search results. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array. Use the variables <a href="../../../varoff/variables/chneventlist1/">ChnEventList1</a>, <a href="../../../varoff/variables/chneventlist2/">ChnEventList2</a>, or <a href="../../../varoff/variables/chneventresultlist/">ChnEventResultList</a> as the return value of this function, or define your own variable.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("[1]/[1]", "[1]/[2]", 40, 50, 0, 0)
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
dd.ChnEventResultList = dd.ChnEventResultAddPrePost(dd.ChnEventResultList, "[1]/[1]", 10, 0, "Value")
dd.ChnEventCreateStatusChn("Event/EventStatusPreTigger", dd.ChnEventResultList, "[1]/[2]", 0, 1)
```

---

*Source: `ComOff/ChnEventResultAddPrePost.htm`*
