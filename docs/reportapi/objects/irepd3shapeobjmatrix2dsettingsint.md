---
title: "IRepD3ShapeObjMatrix2DSettingsInt"
description: "The 3DMatrix2DSettings object provides the curve properties of a 3D axis system in the 2D matrix display mode in DIAdem REPORT."
---

# IRepD3ShapeObjMatrix2DSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DMatrix2DSettings

The 3DMatrix2DSettings object provides the curve properties of a 3D axis system in the 2D matrix display mode in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeMatrix2D, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Dimensions.WidthX = 10
oMySettings.Dimensions.WidthY = 10
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue )
oMySettings.Line.Width = dd.eLineWidth0025
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjmatrix2dsettingsint-dimensions/">Dimensions</a> | <a href="../../properties/irepd3shapeobjmatrix2dsettingsint-filling/">Filling</a> | <a href="../../properties/irepd3shapeobjmatrix2dsettingsint-line/">Line</a> | <a href="../../properties/irepd3shapeobjmatrix2dsettingsint-palette/">Palette</a> | <a href="../../properties/irepd3shapeobjmatrix2dsettingsint-showhiddenlines/">ShowHiddenLines</a> | <a href="../../properties/irepd3shapeobjmatrix2dsettingsint-showzeroheight/">ShowZeroHeight</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobj2dmatrixint/">3DMatrix2D</a>.<a href="../../properties/irepd3shapeobj2dmatrixint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjMatrix2DSettingsInt.htm`*
