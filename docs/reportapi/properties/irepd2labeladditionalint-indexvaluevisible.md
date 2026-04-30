---
title: "IRepD2LabelAdditionalInt.IndexValueVisible"
description: "Specifies whether DIAdem REPORT displays the value index of a 2D curve in the display modes Line and points or Special combination at the curve points."
---

# IRepD2LabelAdditionalInt.IndexValueVisible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndexValueVisible for 2DAdditionalLabel

Specifies whether DIAdem REPORT displays the value index of a 2D curve in the display modes Line and points or Special combination at the curve points.

## Signature

```python
obj.IndexValueVisible
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
oMyChnLabel = oMyCurve.Shape.Extensions.Label
oMyChnLabel.IndexValueVisible = True
oMyChnLabel.IndexValueFormat = "d"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndexValueVisible_IRepD2LabelAdditionalInt.htm`*
