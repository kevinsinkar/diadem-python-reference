---
title: "IRepD3BarDimensionInt"
description: "The 3DBarDimension object provides the displacement and the width of the rectangles and the 3D bars of a 3D axis system in DIAdem REPORT."
---

# IRepD3BarDimensionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DBarDimension

The 3DBarDimension object provides the displacement and the width of the rectangles and the 3D bars of a 3D axis system in DIAdem REPORT.

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
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
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
<p><a href="../../properties/irepd3bardimensionint-offsetx/">OffsetX</a> | <a href="../../properties/irepd3bardimensionint-offsety/">OffsetY</a> | <a href="../../properties/irepd3bardimensionint-widthx/">WidthX</a> | <a href="../../properties/irepd3bardimensionint-widthy/">WidthY</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjbarssettingsint/">3DBarsSettings</a>.<a href="../../properties/irepd3shapeobjbarssettingsint-dimensions/">Dimensions</a> | <a href="../irepd3shapeobjmatrix2dsettingsint/">3DMatrix2DSettings</a>.<a href="../../properties/irepd3shapeobjmatrix2dsettingsint-dimensions/">Dimensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3BarDimensionInt.htm`*
