---
title: "IRepD2SpecialCombAdditionalStylesInt.Offset"
description: "Specifies the displacement of the bars as a percentage in the special display of bars in a 2D axis system in DIAdem REPORT. The entry is a percentage of the max"
---

# IRepD2SpecialCombAdditionalStylesInt.Offset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Offset for 2DAdditionalStyles

Specifies the displacement of the bars as a percentage in the special display of bars in a 2D axis system in DIAdem REPORT. The entry is a percentage of the maximum bar width.

## Signature

```python
obj.Offset
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
oMyAdditionalStyles = oMyShape.Extensions.AdditionalStyles
oMyAdditionalStyles.Type = dd.e2DAdditionalStyleBars
oMyAdditionalStyles.Width = 25
oMyAdditionalStyles.Offset = 0
oMyAdditionalStyles.Line.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyAdditionalStyles.Line.Width = dd.eLineWidth0025
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Offset_IRepD2SpecialCombAdditionalStylesInt.htm`*
