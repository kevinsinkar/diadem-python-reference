---
title: "IRepD2ShapeObjSpecialCombinationExtensionsInt.Label"
description: "Specifies the curve labels in the Special combination display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjSpecialCombinationExtensionsInt.Label

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Label for 2DSpecialCombinationExtensions

Specifies the curve labels in the Special combination display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Label
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\Report_EXPL","TDM","")
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
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Text = "*"
oMyLabel.Repetition.PercentValue = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Label_IRepD2ShapeObjSpecialCombinationExtensionsInt.htm`*
