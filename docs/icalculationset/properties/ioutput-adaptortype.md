---
title: "IOutput.AdaptorType"
description: "Specifies the data type of an output of a calculation."
---

# IOutput.AdaptorType

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: AdaptorType for Output

Specifies the data type of an output of a calculation.

## Signature

```python
obj.AdaptorType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAdaptorTypeValue` | 100 | The output refers to a value. |
| `eAdaptorTypeChannel` | 101 | The output refers to a channel. |
| `eAdaptorTypeChannelList` | 102 | The output refers to a channel list. |

## Python example

```python
oMyOutputs = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs
for I in range( 1, oMyOutputs.Count+1):
    select_variable_0 = oMyOutputs(i).AdaptorType
    if (select_variable_0 == dd.eAdaptorTypeValue) :
        sType = "Value"
    elif (select_variable_0 == dd.eAdaptorTypeChannel) :
        sType = "Channel"
    elif (select_variable_0 == dd.eAdaptorTypeChannelList) :
        sType = "Channel list"
    dd.MsgBoxDisp("Type of " + oMyOutputs(i).Name + " : " + sType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_AdaptorType_IOutput.htm`*
