---
title: "FormulaCalc"
description: "Uses the Calculator AUT syntax to calculate a formula in a script."
---

# FormulaCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FormulaCalc

Uses the Calculator AUT syntax to calculate a formula in a script.

## Signature

```python
dd.FormulaCalc(FormulaTxt)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You can use the <a href="../calculate/">Calculate</a> command to calculate a function in the VBS syntax. Use the <span class="Monospace">Calculate</span> command to include units in quantity-based calculations and to do symbolic replacements. The <span class="Monospace">FormularCalc</span> command ignores the setting of the <a href="../../../varoff/variables/calcquantitybased/">CalcQuantityBased</a> variable and never calculates quantity-based.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the unique definitions for <a href="#" data-unresolved="1">channels and channel references</a> when you calculate with data channels.</td></tr></table>
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
</table>
</div>

## Python example

```python
dd.FormulaCalc("Ch('Group2/Result')() := 2 * 'Group1/Input'")
```

```python
dd.FormulaCalc() ("Ch('Group3/Result'):= Exp('Group1/Input')")
```

---

*Source: `ComOff/FormulaCalc.htm`*
