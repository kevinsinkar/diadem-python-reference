---
title: "IRepD3ShapeObjVectorExtensionsInt"
description: "The 3DVectorExtensions object provides the extended properties of the curve parameters of a 3D axis system in the Vector display mode in DIAdem REPORT."
---

# IRepD3ShapeObjVectorExtensionsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DVectorExtensions

The 3DVectorExtensions object provides the extended properties of the curve parameters of a 3D axis system in the Vector display mode in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeVector, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.VectorType = dd.e3DVectorType6D
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
oMyShape.XChannelEnd.Reference = "[3]/[4]"
oMyShape.YChannelEnd.Reference = "[3]/[5]"
oMyShape.ZChannelEnd.Reference = "[3]/[6]"
oMySettings = oMyShape.Settings
oMySettings.EndCoordinateType = dd.e3DVectorEndCoordinateCartesianRelative
oMySettings.ScalingType = dd.e3DVectorScalingIsometric
oMyArrowHead = oMySettings.ArrowHead
oMyArrowHead.Type = dd.e3DVectorHeadVectorEnd
oMyArrowHead.DynamicSize = True
oMyArrowHead.Size = 15
oMyCurveLineExtension = oMyShape.Extensions.CurveLine
oMyCurveLineExtension.Visible = True
oMyCurveLineExtension.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyCurveLineExtension.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjvectorextensionsint-curveline/">CurveLine</a> | <a href="../../properties/irepd3shapeobjvectorextensionsint-label/">Label</a> | <a href="../../properties/irepd3shapeobjvectorextensionsint-marker/">Marker</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjvectorint/">3DVector</a>.<a href="../../properties/irepd3shapeobjvectorint-extensions/">Extensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjVectorExtensionsInt.htm`*
