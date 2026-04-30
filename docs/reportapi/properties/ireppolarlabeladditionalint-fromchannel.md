---
title: "IRepPolarLabelAdditionalInt.FromChannel"
description: "Specifies whether DIAdem REPORT uses values from another channel for the additional labels of a polar curve in the Lines and points display mode. Assign the val"
---

# IRepPolarLabelAdditionalInt.FromChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FromChannel for PolarAdditionalLabel

Specifies whether DIAdem REPORT uses values from another channel for the additional labels of a polar curve in the Lines and points display mode. Assign the value TRUE to the Visible property so that DIAdem displays the labels from the channel.

## Signature

```python
return_value = obj.FromChannel
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
oMyLabel.IndexValueVisible = True
oMyLabel.IndexValueFormat = "d.dd"
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

*Source: `ReportApi/properties/Report_property_FromChannel_IRepPolarLabelAdditionalInt.htm`*
