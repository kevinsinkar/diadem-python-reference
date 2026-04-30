---
title: "IRepSheetDimensionsInt.Width"
description: "Specifies the width of the current worksheet in DIAdem REPORT. DIAdem REPORT only includes the property Width if you assign the value TRUE to the UseLocalSettin"
---

# IRepSheetDimensionsInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for SheetDimensions

Specifies the width of the current worksheet in DIAdem REPORT. DIAdem REPORT only includes the property Width if you assign the value TRUE to the UseLocalSettings property.

## Signature

```python
obj.Width
```

## Python example

```python
oMyActSheet = dd.Report.ActiveSheet
dd.MsgBoxDisp(oMyActSheet.Dimensions.Width)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepSheetDimensionsInt.htm`*
