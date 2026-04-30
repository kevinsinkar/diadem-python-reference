---
title: "IRepSheetDimensionsInt.Height"
description: "Specifies the height of the current worksheet in DIAdem REPORT. DIAdem only includes the property Height if you assign the value TRUE to the UseLocalSettings pr"
---

# IRepSheetDimensionsInt.Height

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Height for SheetDimensions

Specifies the height of the current worksheet in DIAdem REPORT. DIAdem only includes the property Height if you assign the value TRUE to the UseLocalSettings property.

## Signature

```python
obj.Height
```

## Python example

```python
oMyActDim = dd.Report.ActiveSheet.Dimensions
dd.MsgBoxDisp(oMyActDim.Height)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Height_IRepSheetDimensionsInt.htm`*
