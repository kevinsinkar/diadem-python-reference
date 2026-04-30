---
title: "IRepD2ShapeObjFilledAreaSettingsInt.ConnectNoValueNeighbors"
description: "Specifies whether DIAdem REPORT connects NoValues in curves in the Filled area display mode in a 2D axis system."
---

# IRepD2ShapeObjFilledAreaSettingsInt.ConnectNoValueNeighbors

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ConnectNoValueNeighbors for 2DFilledAreaSettings

Specifies whether DIAdem REPORT connects NoValues in curves in the Filled area display mode in a 2D axis system.

## Signature

```python
obj.ConnectNoValueNeighbors
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeFilledArea, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
oMySettings.FillEffects.Pattern = dd.eFillPatternFilled
oMySettings.ConnectNoValueNeighbors = True
oMySettings.FillEffects.Color.SetPredefinedColor(dd.eColorIndexRed)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ConnectNoValueNeighbors_IRepD2ShapeObjFilledAreaSettingsInt.htm`*
