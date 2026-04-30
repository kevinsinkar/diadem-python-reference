---
title: "IFormulaAdaptor.ReferenceType"
description: "Specifies the reference type, which is dependent on the data type, of the input or output of a calculation."
---

# IFormulaAdaptor.ReferenceType

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: ReferenceType for InputOrOutput

Specifies the reference type, which is dependent on the data type, of the input or output of a calculation.

## Signature

```python
obj.ReferenceType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eReferenceTypeValue` | 110 | The input refers to any value (Value data type). |
| `eReferenceTypeDatasetProperty` | 111 | The input refers to a data set property (Value data type). |
| `eReferenceTypeChannelGroupProperty` | 112 | The input refers to a channel group property (Value data type). |
| `eReferenceTypeChannelProperty` | 113 | The input refers to a channel property (Value data type). |
| `eReferenceTypeChannel` | 114 | The input refers to a channel (Channel data type). |
| `eReferenceTypeChannelList` | 115 | The input refers to a channel list (Channel list data type). |

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_ReferenceType_IFormulaAdaptor.htm`*
