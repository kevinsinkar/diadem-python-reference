---
title: "IRepD2LabelAdditionalInt.IndexValueFormat"
description: "Specifies the format definition for the labeling of a 2D curve with the value index in DIAdem REPORT. You must assign the value TRUE to the property IndexValueV"
---

# IRepD2LabelAdditionalInt.IndexValueFormat

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndexValueFormat for 2DAdditionalLabel

Specifies the format definition for the labeling of a 2D curve with the value index in DIAdem REPORT. You must assign the value TRUE to the property IndexValueVisible in order to use the IndexValueFormat property.

## Signature

```python
obj.IndexValueFormat
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

*Source: `ReportApi/properties/Report_property_IndexValueFormat_IRepD2LabelAdditionalInt.htm`*
