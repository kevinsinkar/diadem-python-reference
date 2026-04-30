---
title: "IRepD3SurfaceIsolineAdditionalInt.DisplayType"
description: "Specifies how DIAdem REPORT displays the additional isolines of a 3D axis system in the Surface display mode in DIAdem REPORT."
---

# IRepD3SurfaceIsolineAdditionalInt.DisplayType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayType for 3DAdditionalSurfaceIsoline

Specifies how DIAdem REPORT displays the additional isolines of a 3D axis system in the Surface display mode in DIAdem REPORT.

## Signature

```python
obj.DisplayType
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        oMyCurves = oMyReportObj.Curves3D
        for oMyCurve in oMyCurves:
            if oMyCurve.ShapeType == dd.e3DShapeSurface :
                oMySurfaceLine = oMyCurve.Shape.Extensions.SurfaceIsoline
                oMySurfaceLine.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected
                oMySurfaceLine.Visible = True
                oMySurfaceLine.Line.Color.ColorIndex = dd.eColorIndexPalette
                oMyColoredLines = oMyCurve.Shape.Settings.Palette
                for i in range( 1, oMyColoredLines.Count+1):
                    oMyColoredLines(i).LineType = dd.eLineTypeDashDot
                    oMyColoredLines(i).Width = dd.eLineWidth0050
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayType_IRepD3SurfaceIsolineAdditionalInt.htm`*
