---
title: "ChnMultipleSortExt"
description: "Sorts the values in data channels. DIAdem sorts texts according to the ASCII table."
---

# ChnMultipleSortExt

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnMultipleSortExt

Sorts the values in data channels. DIAdem sorts texts according to the ASCII table.

## Signature

```python
return_value = dd.ChnMultipleSortExt(ChnList1, ChnList2, MultipleSortExtOrder, MultipleSortExtCaseSensitive, MultipleSortExtIP)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If you do not specify a value for the <span class="Monospace">MultipleSortExtIP</span> variable, DIAdem creates new result channels.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">ChnList2</td>
<td>Specifies one or more channels.<div id="exp_ChnList2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">MultipleSortExtOrder</td>
<td>Specifies whether DIAdem sorts values and text in ascending or descending order.<div id="exp_MultipleSortExtOrder">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">The String variable uses the following script terms:</p>
<table class="Borderless">
<tr>
<td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td>
</tr>
<tr>
<td width="150"><donottranslate><pre>"Up"</pre></donottranslate></td>
<td>Sort in ascending order</td>
</tr>
<tr>
<td width="150"><donottranslate><pre>"Down"</pre></donottranslate></td>
<td>Sort in descending order</td>
</tr>
</table>
<p class="Body">For each control channel you must enter a script term which is separated by a comma. If you use two control channels and define a different sorting order for each channel, the string variable may look as follows: <span class="Monospace">"Down,Up”</span>. If you want to sort both control channels in ascending order, you only need to use a script term: <span class="Monospace">"Up”</span>. If you use more than the two control channels and have only entered two script terms in the <span class="Monospace">MultipleSortExtOrder</span> variable, DIAdem uses the last script term for all other control channels.</p>
</div></td></tr>
<tr><td width="150">MultipleSortExtCaseSensitive</td>
<td>Specifies whether and how DIAdem sorts text case-sensitively.<div id="exp_MultipleSortExtCaseSensitive">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">The String variable uses the following script terms:</p>
<table class="Borderless">
<tr>
<td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td>
</tr>
<tr>
<td width="150"><donottranslate><pre>"CaseInsensitive"</pre></donottranslate></td>
<td>Ignore Upper/Lower Case</td>
</tr>
<tr>
<td width="150"><donottranslate><pre>"UpperCase"</pre></donottranslate></td>
<td>Uppercase First</td>
</tr>
<tr>
<td width="150"><donottranslate><pre>"LowerCase"</pre></donottranslate></td>
<td>Lowercase First</td>
</tr>
</table>
<p class="Body">For each control channel you must enter a script term which is separated by a comma. If you use three control channels and define different case sensitivity for each channel, the string variable may look as follows:<span class="Monospace">"CaseInsensitive,UpperCase,LowerCase"</span>. If you want to sort all three control channels by <span class="Monospace">UpperCase</span>, you only need to use this script term once:<span class="Monospace">"UpperCase"</span>. If you use more than three control channels and have only entered three script terms in the <span class="Monospace">MultipleSortExtCaseSensitive</span> variable, DIAdem uses the last script term for all other control channels.</p>
</div></td></tr>
<tr><td width="150">MultipleSortExtIP</td>
<td>Specifies that DIAdem stores the results in the original channels.<div id="exp_MultipleSortExtIP">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If you do not specify a value for the <span class="Monospace">MultipleSortExtIP</span> variable, DIAdem creates new result channels.</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.Data.Root.Clear()
MyChnGroup1 = dd.Data.Root.ChannelGroups.Add ("Sorted")
MyChnGroup2 = dd.Data.Root.ChannelGroups.Add ("Moved")
MyTextChn1 = MyChnGroup1.Channels.Add("Text", dd.DataTypeString)
MyNumericChn1 = MyChnGroup1.Channels.Add("Numbers", dd.DataTypeChnFloat64)
MyNumericChn2 = MyChnGroup2.Channels.Add("MovedNumbers", dd.DataTypeChnFloat64)
MyTextChn1.Values[1] = "abc"
MyTextChn1.Values[2] = "aBc"
MyTextChn1.Values[3] = "Abc"
MyTextChn1.Values[4] = "Abc"
for I in range( 1, 4+1):
    MyNumericChn1.Values[I] = I
    MyNumericChn2.Values[I] = I

dd.ChnResult = dd.ChnMultipleSortExt(MyChnGroup1.Channels ,MyNumericChn2, "Up,Down", "UpperCase,CaseInsensitive", 0)
```

---

*Source: `ComOff/ChnMultipleSortExt.htm`*
