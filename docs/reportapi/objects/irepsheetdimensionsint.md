---
title: "IRepSheetDimensionsInt"
description: "The SheetDimensions object provides the properties of the page format in DIAdem REPORT."
---

# IRepSheetDimensionsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SheetDimensions

The SheetDimensions object provides the properties of the page format in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsheetdimensionsint-height/">Height</a> | <a href="../../properties/irepsheetdimensionsint-orientation/">Orientation</a> | <a href="../../properties/irepsheetdimensionsint-ratio/">Ratio</a> | <a href="../../properties/irepsheetdimensionsint-uselocalsettings/">UseLocalSettings</a> | <a href="../../properties/irepsheetdimensionsint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsheetint/">Sheet</a>.<a href="../../properties/irepsheetint-dimensions/">Dimensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSheetDimensionsInt.htm`*
