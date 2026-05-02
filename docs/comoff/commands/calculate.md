---
title: "Calculate"
description: "Uses the Calculator formula syntax to calculate a formula in a script including the units."
---

# Calculate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: Calculate

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.BoolVarSet('CalcQuantityBased', ...)   # instead of dd.CalcQuantityBased = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Uses the Calculator formula syntax to calculate a formula in a script including the units.

## Signature

```python
dd.Calculate(CalculateFormula, [CalculateSymbols], [CalculateValues], [CalculateTargetUnit])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CalculateFormula</td>
<td>Specifies a formula in a script. Enter the formula in quotation marks. You must enclose texts that are in quotation marks, such as channel names, in double quotation marks.<div id="exp_CalculateFormula">
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
<tr><td width="150">[CalculateTargetUnit]</td>
<td>Specifies the unit symbol for the result of the calculation. If you do not specify a unit symbol, DIAdem specifies the unit symbol.<div id="exp_CalculateTargetUnit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.Calculate("Ch(\"Group2/Result\")= 2 * Ch(\"Group1/Input\")")
```

```python
dd.Calculate("Ch(\"Group3/Result\")= Exp(Ch(\"Group1/Input\"))")
```

```python
sFormula = "R1 = A / B"
aSymbol = []
aSymbol.append("A")
aSymbol.append("B")
aValues = []
aValues.append(2)
aValues.append(3)
dd.Calculate (sFormula, aSymbol, aValues)
dd.MsgboxDisp(dd.R1)
```

```python
sFormula = "Ch(\"Result\") = A / B"
aSymbol = []
aSymbol.append("A")
aSymbol.append("B")
aValues = []
aValues.append(dd.Data.GetChannel("[1]/[2]"))
aValues.append(dd.Data.GetChannel("[1]/[3]"))
dd.Calculate (sFormula, aSymbol, aValues)
```

```python
sFormula = "Ch(\"Result\") = A / len(\"B\")"
aSymbol = []
aSymbol.append("A")
aSymbol.append("B")
aValues = []
aValues.append(dd.Data.GetChannel("[1]/[2]"))
aValues.append("Example Text")
dd.Calculate (sFormula, aSymbol, aValues)
```

```python
dd.CalcQuantityBased = True
dd.Calculate("r1=vu(10,\"m\")+vu(2,\"cm\")",None ,None ,"in")
dd.MsgboxDisp("Result: " +  dd.R1 + "\r\n" + "Unit: " + dd.CalculateResultUnit)
dd.Calculate("r1=vu(10,\"m\")+vu(2,\"cm\")","default")
dd.MsgboxDisp("Result: " +  dd.R1 + "\r\n" + "Unit: " + dd.CalculateResultUnit)
```

```python
sFormula = "C= A + B"
aSymbol = []
aSymbol.append("A")
aSymbol.append("B")
aSymbol.append("C")
aMyValueUnit = []
aMyValueUnit.append(dd.CreateValueWithUnit(10, "m"))
aMyValueUnit.append(dd.CreateValueWithUnit(2, "cm"))
aMyValueUnit.append(dd.CreateValueWithUnit(None, ""))
dd.Calculate (sFormula, aSymbol, aMyValueUnit, "default")
dd.MsgboxDisp("Result: " +  aMyValueUnit(3).Value + "\r\n" + "Unit: " + aMyValueUnit(3).UnitSymbol)
```

---

*Source: `ComOff/Calculate.htm`*
