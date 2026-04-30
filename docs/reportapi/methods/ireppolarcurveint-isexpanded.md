---
title: "IRepPolarCurveInt.IsExpanded"
description: "Specifies whether a curve in a polar axis system in DIAdem REPORT is expanded. You must not change the channel reference of an expanded curve. You may only chan"
---

# IRepPolarCurveInt.IsExpanded

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: IsExpanded for PolarCurve

Specifies whether a curve in a polar axis system in DIAdem REPORT is expanded. You must not change the channel reference of an expanded curve. You may only change the channel reference if the curve is a PolarCurveDrawingContext object.

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
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        oMyCurves = oMyReportObj.CurvesPolar
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

*Source: `ReportApi/methods/Report_method_IsExpanded_IRepPolarCurveInt.htm`*
