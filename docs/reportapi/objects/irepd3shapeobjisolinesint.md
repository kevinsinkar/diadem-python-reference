---
title: "IRepD3ShapeObjIsolinesInt"
description: "The 3DIsolines object provides the curve properties of a 3D axis system in the Isolines display mode in DIAdem REPORT."
---

# IRepD3ShapeObjIsolinesInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DIsolines

The 3DIsolines object provides the curve properties of a 3D axis system in the Isolines display mode in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.IsolineType = dd.e3DIsolineTypeXY
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjisolinesint-extensions/">Extensions</a> | <a href="../../properties/irepd3shapeobjisolinesint-isolinetype/">IsolineType</a> | <a href="../../properties/irepd3shapeobjisolinesint-numberofisochannels/">NumberOfIsoChannels</a> | <a href="../../properties/irepd3shapeobjisolinesint-settings/">Settings</a> | <a href="../../properties/irepd3shapeobjisolinesint-xchannel/">XChannel</a> | <a href="../../properties/irepd3shapeobjisolinesint-ychannel/">YChannel</a> | <a href="../../properties/irepd3shapeobjisolinesint-zchannel/">ZChannel</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjIsolinesInt.htm`*
