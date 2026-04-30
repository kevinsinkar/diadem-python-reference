---
title: "IRepErrorBarInt.PercentageErrorValue"
description: "Specifies the percentage error value of a 2D curve in DIAdem REPORT."
---

# IRepErrorBarInt.PercentageErrorValue

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PercentageErrorValue for ErrorBar

Specifies the percentage error value of a 2D curve in DIAdem REPORT.

## Signature

```python
obj.PercentageErrorValue
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        for oMyCurve in oMyReportObj.Curves2D:
            if oMyCurve.ShapeType == dd.e2DShapeLine or oMyCurve.ShapeType == dd.e2DShapeLineAndPoints or oMyCurve.ShapeType == dd.e2DShapeSpecialCombination :
                dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Error value: " + oMyCurve.Shape.Extensions.ErrorBars.XErrorBar.PercentageErrorValue)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PercentageErrorValue_IRepErrorBarInt.htm`*
