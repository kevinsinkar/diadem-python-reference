---
title: "ChnResultUnitGet"
description: "Returns the symbol of the result unit if you perform an arithmetic operation on a channel."
---

# ChnResultUnitGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnResultUnitGet

Returns the symbol of the result unit if you perform an arithmetic operation on a channel.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">ChnUnitOperator</td>
<td>Specifies the operator.<div id="exp_ChnUnitOperator">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"PlusMinus"</pre></donottranslate></td>
<td>Add/Subtract</td></tr>
<tr><td width="150"><donottranslate><pre>"Multiply"</pre></donottranslate></td>
<td>Multiply</td></tr>
<tr><td width="150"><donottranslate><pre>"Divide"</pre></donottranslate></td>
<td>Divide</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String variable</a> type.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnResultUnitGet.htm`*
