---
title: "IRepD3LabelIsolineAdditionalInt.UseCurveColor"
description: "Specifies whether DIAdem REPORT uses the same line color for the lines and the labeling of the isolines."
---

# IRepD3LabelIsolineAdditionalInt.UseCurveColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCurveColor for 3DAdditionalIsolineLabel

Specifies whether DIAdem REPORT uses the same line color for the lines and the labeling of the isolines.

## Signature

```python
obj.UseCurveColor
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
oMyLabel = oMyShape.Extensions.IsolineLabel
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.d"
oMyLabel.UseCurveColor = False
oMyLabel.Font.Color.ColorIndex = dd.eColorIndexBlue
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCurveColor_IRepD3LabelIsolineAdditionalInt.htm`*
