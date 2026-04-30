---
title: "IRepD3IsolinesCountExpInt.Count"
description: "Changes the number of isolines for the 3D display mode Isolines in DIAdem REPORT or returns this value."
---

# IRepD3IsolinesCountExpInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 3DIsolinesCountObject

Changes the number of isolines for the 3D display mode Isolines in DIAdem REPORT or returns this value.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        oMyCurves = oMyReportObj.Curves3D
        for oMyCurve in oMyCurves:
            if oMyCurve.ShapeType == dd.e3DShapeIsolines :
                oMyCurve.Shape.NumberOfIsoChannels.Count = 5
                dd.MsgBoxDisp("Number of isolines: " + oMyCurve.Shape.NumberOfIsoChannels.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepD3IsolinesCountExpInt.htm`*
