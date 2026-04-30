---
title: "ChnFind"
description: "Determines the first row in a data channel that meets a specified condition. The ChnFind function searches a data channel from the beginning to the end."
---

# ChnFind

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFind

Determines the first row in a data channel that meets a specified condition. The ChnFind function searches a data channel from the beginning to the end.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the commands <a href="../valequal/">ValEqual</a>, <a href="../valequallt/">ValEqualLT</a>, or <a href="../valequalgt/">ValEqualGT</a> if you want to check whether two real numbers are equal, smaller than or equal, or greater than or equal. DIAdem uses only the significant digits of a number in these commands. The <span class="Monospace">ChnFind</span> command does not operate quantity-based therefore it cannot work with value-unit objects such as the <a href="#" data-unresolved="1">VU</a> function.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FormulaTxt</td>
<td>Specifies a formula in a script. Enter the formula in quotation marks. You must enclose texts that are in quotation marks, such as channel names, in double quotation marks.<div id="exp_FormulaTxt">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnFindStartIdx]</td>
<td>Specifies the row number at which DIAdem begins checking the data channel for a condition. By default DIAdem checks the data channel in the <span class="Monospace">ChnFind</span> command from the first row and in the <span class="Monospace">ChnFindReverse</span> command from the last row.<div id="exp_ChnFindStartIdx">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= ChnFindStartIdx &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">[CalculateSymbols]</td>
<td>Specifies a list with symbol names, which are replaced in the formula with values. The symbols <span class="Monospace">CalculateSymbols</span> and the values <span class="Monospace">CalculateValues</span> are assigned through their field index.<div id="exp_CalculateSymbols">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[CalculateValues]</td>
<td>Specifies a list of the values associated with the symbols. The symbols <span class="Monospace">CalculateSymbols</span> and the values <span class="Monospace">CalculateValues</span> are assigned through their field index.<div id="exp_CalculateValues">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p>The <span class="Monospace">CalculateValues</span> vector can contain numeric values, texts, <a href="../../../ivalueunit/objects/ivalueunit/">Value-Unit objects</a>, and <a href="../../../inavidata/objects/idiademchannel/">Channel objects</a>. DIAdem interprets the value-unit objects like the <a href="#" data-unresolved="1">VU</a> function and channel objects like the <a href="../../../varoff/variables/ch/">Ch</a> variable.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is an <a href="#" data-unresolved="1">Integer variable</a> type. Returns the first row number that satisfies the given condition. If no row of the data channel meets the condition, the <span class="Monospace">ChnFind</span> command returns the result <span class="Monospace">0</span>. If the <span class="Monospace">ChnFindStartIdx</span> variable is longer than the channel, the <span class="Monospace">ChnFind</span> command returns the result <span class="Monospace">0</span>. If the channel is empty, the <span class="Monospace">ChnFind</span> command returns the result -1.</td></tr>
</table>
</div>

## Python example

```python
intMyResult = dd.ChnFind("Ch(\"Group1/Channel\")>10",250)
```

```python
print(dd.ChnFind("instr(1,ch(\"Group1/Textchannel\"),\"meas\",1)0"))
```

```python
sFormula = "A >= B"
aSymbol = []
aSymbol.append("A")
aSymbol.append("B")
aValues = []
aValues.append(dd.Data.GetChannel("[1]/[1]"))
aValues.append(30)
print(dd.ChnFind(sFormula,None ,aSymbol, aValues))
```

---

*Source: `ComOff/ChnFind.htm`*
