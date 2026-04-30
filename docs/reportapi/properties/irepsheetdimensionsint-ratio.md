---
title: "IRepSheetDimensionsInt.Ratio"
description: "Returns the ratio of page height to page width for the current worksheet in DIAdem REPORT. DIAdem only includes the Ratio property if you assign the value TRUE "
---

# IRepSheetDimensionsInt.Ratio

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Ratio for SheetDimensions

Returns the ratio of page height to page width for the current worksheet in DIAdem REPORT. DIAdem only includes the Ratio property if you assign the value TRUE to the UseLocalSettings property.

## Signature

```python
obj.Ratio
```

## Python example

```python
oMyDimensions = dd.Report.Settings.Page.Dimensions
oMyDimensions.UseScaledOutput = False
oMyDimensions.Ratio = 1.5

oMySheetDimension = dd.Report.ActiveSheet.Dimensions
oMySheetDimension.UseLocalSettings = True
oMySheetDimension.Orientation = dd.ePageOrientationLandscape
dd.MsgBoxDisp(oMySheetDimension.Ratio)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Ratio_IRepSheetDimensionsInt.htm`*
