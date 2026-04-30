---
title: "IRepD3IsoValueTableListInt.Count"
description: "Changes the number of isolines in the contour table for the 3D display mode Characteristic diagram in DIAdem REPORT or returns this value."
---

# IRepD3IsoValueTableListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 3DIsoValueTable

Changes the number of isolines in the contour table for the 3D display mode Characteristic diagram in DIAdem REPORT or returns this value.

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
            if oMyCurve.ShapeType == dd.e3DShapeCharacteristicDiagram :
                dd.MsgBoxDisp("Number of isolines: " + oMyCurve.Shape.Settings.IsoValueTable.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepD3IsoValueTableListInt.htm`*
