---
title: "IRepD3ShapeObjSurfaceInt"
description: "The 3DSurface object provides the curve properties of a 3D axis system in the Surface display mode in DIAdem REPORT."
---

# IRepD3ShapeObjSurfaceInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DSurface

The 3DSurface object provides the curve properties of a 3D axis system in the Surface display mode in DIAdem REPORT.

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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjsurfaceint-datastructure/">DataStructure</a> | <a href="../../properties/irepd3shapeobjsurfaceint-extensions/">Extensions</a> | <a href="../../properties/irepd3shapeobjsurfaceint-referenceplanezvalue/">ReferencePlaneZValue</a> | <a href="../../properties/irepd3shapeobjsurfaceint-settings/">Settings</a> | <a href="../../properties/irepd3shapeobjsurfaceint-surfaceredundancymode/">SurfaceRedundancyMode</a> | <a href="../../properties/irepd3shapeobjsurfaceint-xchannel/">XChannel</a> | <a href="../../properties/irepd3shapeobjsurfaceint-ychannel/">YChannel</a> | <a href="../../properties/irepd3shapeobjsurfaceint-zchannel/">ZChannel</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3curveint/">3DCurve</a>.<a href="../../properties/irepd3curveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjSurfaceInt.htm`*
