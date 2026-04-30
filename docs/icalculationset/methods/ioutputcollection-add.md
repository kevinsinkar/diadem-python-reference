---
title: "IOutputCollection.Add"
description: "Adds a new output to the Outputs collection and returns an Output object."
---

# IOutputCollection.Add

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Add for Outputs

Adds a new output to the Outputs collection and returns an Output object.

## Signature

```python
return_value = obj.Add(Name, AdaptorType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAdaptorTypeValue` | 100 | The output refers to a value. |
| `eAdaptorTypeChannel` | 101 | The output refers to a channel. |
| `eAdaptorTypeChannelList` | 102 | The output refers to a channel list. |

## Python example

```python
oMyCalcTemp = dd.CalculationSet.CalculationGroups("Custom").Calculations(1)
if not oMyCalcTemp.Outputs.Exists("R") :
    oMyCalcTemp.Outputs.Add("R", dd.eAdaptorTypeChannel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Add_IOutputCollection.htm`*
