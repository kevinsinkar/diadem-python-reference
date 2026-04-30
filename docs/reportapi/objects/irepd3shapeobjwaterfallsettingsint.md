---
title: "IRepD3ShapeObjWaterfallSettingsInt"
description: "The 3DWaterfallSettings object provides the properties of the curve parameters in a 3D axis system in the Waterfall display mode in DIAdem REPORT."
---

# IRepD3ShapeObjWaterfallSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DWaterfallSettings

The 3DWaterfallSettings object provides the properties of the curve parameters in a 3D axis system in the Waterfall display mode in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeWaterfall, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue )
oMySettings.Line.Width = dd.eLineWidth0100
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjwaterfallsettingsint-line/">Line</a> | <a href="../../properties/irepd3shapeobjwaterfallsettingsint-palette/">Palette</a> | <a href="../../properties/irepd3shapeobjwaterfallsettingsint-showhiddenlines/">ShowHiddenLines</a> | <a href="../../properties/irepd3shapeobjwaterfallsettingsint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjwaterfallint/">3DWaterfall</a>.<a href="../../properties/irepd3shapeobjwaterfallint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjWaterfallSettingsInt.htm`*
