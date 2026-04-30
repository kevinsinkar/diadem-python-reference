---
title: "IRepPolarLabelAdditionalInt.YValueFormat"
description: "Specifies the format definition for labeling a polar curve with its y-values in a polar axis system in the Line and points display mode in DIAdem REPORT. Assign"
---

# IRepPolarLabelAdditionalInt.YValueFormat

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YValueFormat for PolarAdditionalLabel

Specifies the format definition for labeling a polar curve with its y-values in a polar axis system in the Line and points display mode in DIAdem REPORT. Assign the value TRUE to the YValueVisible property so that DIAdem REPORT displays the y-values.

## Signature

```python
obj.YValueFormat
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "PolarSystem")
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
oMyLabel.RelativePosition = dd.eRelativePositionLeft
oMyLabel.Repetition.Mode = dd.eLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YValueFormat_IRepPolarLabelAdditionalInt.htm`*
