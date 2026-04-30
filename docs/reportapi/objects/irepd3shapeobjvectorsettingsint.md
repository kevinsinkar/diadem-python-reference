---
title: "IRepD3ShapeObjVectorSettingsInt"
description: "The 3DVectorSettings object provides the curve properties of a 3D axis system in the Vector display mode in DIAdem REPORT."
---

# IRepD3ShapeObjVectorSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DVectorSettings

The 3DVectorSettings object provides the curve properties of a 3D axis system in the Vector display mode in DIAdem REPORT.

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
<p><a href="../../properties/irepd3shapeobjvectorsettingsint-arrowhead/">ArrowHead</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-endcoordinateangleunit/">EndCoordinateAngleUnit</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-endcoordinatetype/">EndCoordinateType</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-line/">Line</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-palette/">Palette</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-plane4dtype/">Plane4DType</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-plane6dtype/">Plane6DType</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-planethirdcomponenttype/">PlaneThirdComponentType</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-planethirdcomponentvalue/">PlaneThirdComponentValue</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-scalingfactor/">ScalingFactor</a> | <a href="../../properties/irepd3shapeobjvectorsettingsint-scalingtype/">ScalingType</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjvectorint/">3DVector</a>.<a href="../../properties/irepd3shapeobjvectorint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjVectorSettingsInt.htm`*
