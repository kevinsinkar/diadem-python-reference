---
title: "IRepD2ShapeObjOutlBarsSettingsInt.Type"
description: "Specifies whether DIAdem REPORT plots the outlines as stairs or bars in a 2D axis system in the Outlined bars display mode."
---

# IRepD2ShapeObjOutlBarsSettingsInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 2DOutlineBarsSettings

Specifies whether DIAdem REPORT plots the outlines as stairs or bars in a 2D axis system in the Outlined bars display mode.

## Signature

```python
obj.Type
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"
oMySettings = oMyShape.Settings
oMySettings.Type = dd.e2DOutlineBarTypeStairs
oMySettings.Line.Width = dd.eLineWidth0200
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD2ShapeObjOutlBarsSettingsInt.htm`*
