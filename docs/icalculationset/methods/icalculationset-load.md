---
title: "ICalculationSet.Load"
description: "Loads a calculation set from a file that has the filename extension .tca . In doing so, DIAdem overwrites any existing calculation set. If the calculation set f"
---

# ICalculationSet.Load

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Load for CalculationSet

Loads a calculation set from a file that has the filename extension .tca . In doing so, DIAdem overwrites any existing calculation set. If the calculation set file to be loaded is encrypted, you can execute the calculations that the file contains. However you cannot view or edit the calculations.

## Signature

```python
obj.Load(FileName)
```

## Python example

```python
dd.CalculationSet.Load("MyCalculationSet.tca")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Load_ICalculationSet.htm`*
