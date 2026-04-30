---
title: "IRepD3ShapeObjVectorInt.XChannelEnd"
description: "Specifies the x-channel for the end points of a curve in a 3D axis system in the Vector display mode in DIAdem REPORT."
---

# IRepD3ShapeObjVectorInt.XChannelEnd

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XChannelEnd for 3DVector

Specifies the x-channel for the end points of a curve in a 3D axis system in the Vector display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.XChannelEnd
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
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
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XChannelEnd_IRepD3ShapeObjVectorInt.htm`*
