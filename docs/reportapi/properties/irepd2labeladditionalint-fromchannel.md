---
title: "IRepD2LabelAdditionalInt.FromChannel"
description: "Specifies whether DIAdem REPORT uses values from another channel for the additional labels of a 2D curve in the display modes Line and points or Special combina"
---

# IRepD2LabelAdditionalInt.FromChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FromChannel for 2DAdditionalLabel

Specifies whether DIAdem REPORT uses values from another channel for the additional labels of a 2D curve in the display modes Line and points or Special combination . Assign the value TRUE to the Visible property so that DIAdem REPORT displays the values.

## Signature

```python
return_value = obj.FromChannel
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[6]/[1]"
oMyCurve.Shape.YChannel.Reference = "[6]/[2]"
oMyChnLabel = oMyCurve.Shape.Extensions.Label.FromChannel
oMyChnLabel.Channel.Reference = "[7]/[1]"
oMyChnLabel.Visible = True
oMyChnLabel.IndexChannel.Reference = "[6]/[3]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FromChannel_IRepD2LabelAdditionalInt.htm`*
