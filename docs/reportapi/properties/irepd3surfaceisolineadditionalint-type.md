---
title: "IRepD3SurfaceIsolineAdditionalInt.Type"
description: "Specifies the origin of the isovalues of the additional isolines in 3D axis systems in the Surface display mode in DIAdem REPORT."
---

# IRepD3SurfaceIsolineAdditionalInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 3DAdditionalSurfaceIsoline

Specifies the origin of the isovalues of the additional isolines in 3D axis systems in the Surface display mode in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySurfaceIsoline = oMyShape.Extensions.SurfaceIsoline
oMySurfaceIsoline.Type = dd.e3DSurfaceIsoValueCalculated
oMySurfaceIsoline.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected
oMySurfaceIsoline.Visible = True
oMySurfaceIsoline.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColoredLines = oMyShape.Settings.Palette
for i in range( 1, oMyColoredLines.Count+1):
    oMyColoredLines(i).LineType = dd.eLineTypeDashDot
    oMyColoredLines(i).Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD3SurfaceIsolineAdditionalInt.htm`*
