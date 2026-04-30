---
title: "IRepD3PaletteColoredLineListInt.Count"
description: "Returns the number of color ranges for the line color Palette in a 3D axis system in DIAdem REPORT."
---

# IRepD3PaletteColoredLineListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 3DPaletteColoredLines

Returns the number of color ranges for the line color Palette in a 3D axis system in DIAdem REPORT.

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
            if oMyCurve.ShapeType != dd.e3DShapeCharacteristicDiagram :
                dd.MsgBoxDisp("Number of isolines: " + oMyCurve.Shape.Settings.Palette.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepD3PaletteColoredLineListInt.htm`*
