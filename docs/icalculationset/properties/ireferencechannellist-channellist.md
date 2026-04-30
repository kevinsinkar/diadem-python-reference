---
title: "IReferenceChannelList.ChannelList"
description: "Specifies the channel list with which DIAdem replaces an input or an output when a calculation is executed. In channel list references you can use wildcards for"
---

# IReferenceChannelList.ChannelList

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: ChannelList for ReferenceChannelList

Specifies the channel list with which DIAdem replaces an input or an output when a calculation is executed. In channel list references you can use wildcards for group names and channel names. Use a question mark (?) as a wildcard for one character, and an asterisk (*) as a wildcard for any number of characters. The wildcards question mark and asterisk must not be used in the terms in brackets [Group index] and [Channel index] . Click here for further information about the syntax of channel lists. You can add the contents of a DIAdem variable or a calculator expression to the channel group property if you enclose the variable or the calculator expression in @@ characters. If the input of the calculation is dependent on an output from another calculation, you cannot change the ChannelList property.

## Signature

```python
obj.ChannelList
```

## Python example

```python
dd.CalculationSet.CalculationGroups.Item(1).Calculations.Item(1).Inputs.RemoveAll()
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeChannelList)
oMyInput.ReferenceType = dd.eReferenceTypeChannelList
oMyInput.Reference.ChannelList = "'Res_1'-'Res_5'"
for oInputChannel in oMyInput.Reference.ChannelList:
    print(oInputChannel.Name)
```

```python
dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.RemoveAll()
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeChannelList)
oMyInput.ReferenceType = dd.eReferenceTypeChannelList
oMyInput.Reference.ChannelList = "Temp*"
print(oMyInput.Reference.ChannelList)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_ChannelList_IReferenceChannelList.htm`*
