---
title: "IRepD2SpecialCombAdditionalStylesInt.Filling"
description: "Specifies the filling properties of special types in the Special combination display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2SpecialCombAdditionalStylesInt.Filling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Filling for 2DAdditionalStyles

Specifies the filling properties of special types in the Special combination display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Filling
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySettings = oMyShape.Settings
oMyShape.Extensions.AdditionalStyles.Type = dd.e2DAdditionalStyleBars
oMyShape.Extensions.AdditionalStyles.Filling.Color.SetPredefinedColor(dd.ePredefinedColorBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Filling_IRepD2SpecialCombAdditionalStylesInt.htm`*
