---
title: "IRepSheetDimensionsInt.UseLocalSettings"
description: "Specifies whether a DIAdem REPORT worksheet uses the local or the global page format."
---

# IRepSheetDimensionsInt.UseLocalSettings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseLocalSettings for SheetDimensions

Specifies whether a DIAdem REPORT worksheet uses the local or the global page format.

## Signature

```python
obj.UseLocalSettings
```

## Python example

```python
oMyDimensions = dd.Report.Settings.Page.Dimensions
oMyDimensions.UseScaledOutput = False
oMyDimensions.Ratio = 1.5

oMySheetDimension = dd.Report.ActiveSheet.Dimensions
oMySheetDimension.Orientation = dd.ePageOrientationLandscape
oMySheetDimension.UseLocalSettings = True
dd.MsgBoxDisp(oMySheetDimension.Ratio)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseLocalSettings_IRepSheetDimensionsInt.htm`*
