---
title: "IRepPolarLabelAdditionalInt.Font"
description: "Specifies the properties of the curve labels in the Line and points display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarLabelAdditionalInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for PolarAdditionalLabel

Specifies the properties of the curve labels in the Line and points display mode in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyLabel = oMyCurve.Shape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.Font.Name = "Arial"
oMyLabel.RelativePosition = dd.eRelativePositionPointCenter
oMyLabel.Repetition.Mode = dd.eLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepPolarLabelAdditionalInt.htm`*
