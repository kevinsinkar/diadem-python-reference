---
title: "ICalculationSet.Export"
description: "Exports all or selected calculations into a calculation set file ( *.tca )."
---

# ICalculationSet.Export

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Export for CalculationSet

Exports all or selected calculations into a calculation set file ( *.tca ).

## Signature

```python
obj.Export(FileName, [CalculationSelection], [ExportMode])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table3">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  When you save the encrypted calculation, you cannot overwrite an existing file. Always save the unencrypted calculations, because you cannot decrypt a file once it is encrypted.</td>
</tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCalculationAll` | 120 | DIAdem saves all calculations. |
| `eCalculationSelection` | 121 | DIAdem saves only the selected calculations The Selected property specifies whether a calculation is selected. A dependent input loses its dependency when it is saved if you do not save the associated output as well. |
| `eExportModeStandard` | 130 | DIAdem saves the calculation unencrypted. |
| `eExportModeCrypted` | 131 | DIAdem saves the calculation encrypted. |

## Python example

```python
dd.CalculationSet.Export("MyCalculationSet.tca", dd.eCalculationAll)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Export_ICalculationSet.htm`*
