---
title: "IRepD2ShapeObjSpecialCombinationExtensionsInt.ErrorBars"
description: "Returns an error bar for the Special combination curve type in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjSpecialCombinationExtensionsInt.ErrorBars

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ErrorBars for 2DSpecialCombinationExtensions

Returns an error bar for the Special combination curve type in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.ErrorBars
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        for oMyCurve in oMyReportObj.Curves2D:
            if oMyCurve.ShapeType == dd.e2DShapeSpecialCombination :
                dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Channel number: " + oMyCurve.Shape.Extensions.ErrorBars.XErrorBar.Type)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ErrorBars_IRepD2ShapeObjSpecialCombinationExtensionsInt.htm`*
