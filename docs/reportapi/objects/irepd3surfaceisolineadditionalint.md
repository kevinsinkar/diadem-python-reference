---
title: "IRepD3SurfaceIsolineAdditionalInt"
description: "The 3DAdditionalSurfaceIsoline object provides the curve properties of the additional isolines in 3D axis systems in the Surface display mode in DIAdem REPORT."
---

# IRepD3SurfaceIsolineAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalSurfaceIsoline

The 3DAdditionalSurfaceIsoline object provides the curve properties of the additional isolines in 3D axis systems in the Surface display mode in DIAdem REPORT.

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
oMyShape.Extensions.SurfaceIsoline.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected
oMyShape.Extensions.SurfaceIsoline.Visible = True
oMyShape.Extensions.SurfaceIsoline.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColoredLines = oMyShape.Settings.Palette
for i in range( 1, oMyColoredLines.Count+1):
    oMyColoredLines(i).LineType = dd.eLineTypeDashDot
    oMyColoredLines(i).Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3surfaceisolineadditionalint-channel/">Channel</a> | <a href="../../properties/irepd3surfaceisolineadditionalint-displaytype/">DisplayType</a> | <a href="../../properties/irepd3surfaceisolineadditionalint-label/">Label</a> | <a href="../../properties/irepd3surfaceisolineadditionalint-line/">Line</a> | <a href="../../properties/irepd3surfaceisolineadditionalint-type/">Type</a> | <a href="../../properties/irepd3surfaceisolineadditionalint-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjsurfaceextensionsint/">3DSurfaceExtensions</a>.<a href="../../properties/irepd3shapeobjsurfaceextensionsint-surfaceisoline/">SurfaceIsoline</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3SurfaceIsolineAdditionalInt.htm`*
