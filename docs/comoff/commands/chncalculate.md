---
title: "ChnCalculate"
description: "Uses the Calculator VBS syntax to calculate a formula in a script."
---

# ChnCalculate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnCalculate

Uses the Calculator VBS syntax to calculate a formula in a script.

## Signature

```python
dd.ChnCalculate(FormulaTxt)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../calculate/">Calculate</a> command to include units in quantity-based calculations and to replace symbols with values in formulas.</td></tr></table>
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
dd.ChnCalculate("Ch(\"Group2/Result\")= 2 * Ch(\"Group1/Input\")")
```

```python
dd.ChnCalculate("Ch(\"Group3/Result\")= Exp(Ch(\"Group1/Input\"))")
```

---

*Source: `ComOff/ChnCalculate.htm`*
