---
title: "IRepD2ShapeObjSpecialCombinationInt.Extensions"
description: "Specifies the extended properties of a curve in the Special combination display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjSpecialCombinationInt.Extensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Extensions for 2DSpecialCombination

Specifies the extended properties of a curve in the Special combination display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Extensions
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
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
oMyExtension = oMyCurve.Shape.Extensions
oMyExtension.Label.YValueVisible = True
oMyExtension.Label.YValueFormat = "d.dd"
oMyExtension.Label.Position.Type = dd.e2DLabelPositionAtPoint
oMyExtension.Label.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyExtension.Label.Repetition.NValue = 10
oMyExtension.AdditionalStyles.Type = dd.e2DAdditionalStyleSpikes
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Extensions_IRepD2ShapeObjSpecialCombinationInt.htm`*
