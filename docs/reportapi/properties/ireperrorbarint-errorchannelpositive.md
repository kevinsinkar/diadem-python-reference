---
title: "IRepErrorBarInt.ErrorChannelPositive"
description: "Returns the channel reference of an error bar in positive direction in a 2D axis system in DIAdem REPORT."
---

# IRepErrorBarInt.ErrorChannelPositive

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ErrorChannelPositive for ErrorBar

Returns the channel reference of an error bar in positive direction in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.ErrorChannelPositive
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        for oMyCurve in oMyReportObj.Curves2D:
            if oMyCurve.ShapeType == dd.e2DShapeLine or oMyCurve.ShapeType == dd.e2DShapeLineAndPoints or oMyCurve.ShapeType == dd.e2DShapeSpecialCombination :
                dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Channel number: " + oMyCurve.Shape.Extensions.ErrorBars.XErrorBar.ErrorChannelPositve.Reference)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ErrorChannelPositive_IRepErrorBarInt.htm`*
