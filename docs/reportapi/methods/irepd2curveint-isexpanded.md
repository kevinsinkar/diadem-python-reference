---
title: "IRepD2CurveInt.IsExpanded"
description: "Specifies whether a curve in a 2D axis system in DIAdem REPORT is expanded. You must not change the channel reference of an expanded curve. You can only change "
---

# IRepD2CurveInt.IsExpanded

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: IsExpanded for 2DCurve

Specifies whether a curve in a 2D axis system in DIAdem REPORT is expanded. You must not change the channel reference of an expanded curve. You can only change the channel reference if the curve is a D2CurveDrawingContext object.

## Signature

```python
bIsExpanded = Object.IsExpanded()
```

## Python example

```python
sOutput = ""
dd.Report.Settings.CurveExpansion.Expand()
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyCurves = oMyReportObj.Curves2D
        print ("Number of curves: " , oMyCurves.Count)
        for oMyCurve in oMyCurves:
            sOutput = sOutput + "Object index: " + oMyCurve.Index + "\t" + "IsExpanded: " + oMyCurve.IsExpanded + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_IsExpanded_IRepD2CurveInt.htm`*
