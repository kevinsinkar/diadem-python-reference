---
title: "IRepD3ShapeObjLineInt"
description: "The 3DLine object provides the curve properties of a 3D axis system in the 3D curve display mode in DIAdem REPORT."
---

# IRepD3ShapeObjLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DLine

The 3DLine object provides the curve properties of a 3D axis system in the 3D curve display mode in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjlineint-extensions/">Extensions</a> | <a href="../../properties/irepd3shapeobjlineint-settings/">Settings</a> | <a href="../../properties/irepd3shapeobjlineint-xchannel/">XChannel</a> | <a href="../../properties/irepd3shapeobjlineint-ychannel/">YChannel</a> | <a href="../../properties/irepd3shapeobjlineint-zchannel/">ZChannel</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjLineInt.htm`*
