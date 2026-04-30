---
title: "IRepD3LabelIsolineAdditionalInt.IndexValueFormat"
description: "Specifies, in DIAdem REPORT, the format definition for the labeling of a 3D curve in the Isolines display mode with the value index. You must assign the value T"
---

# IRepD3LabelIsolineAdditionalInt.IndexValueFormat

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndexValueFormat for 3DAdditionalIsolineLabel

Specifies, in DIAdem REPORT, the format definition for the labeling of a 3D curve in the Isolines display mode with the value index. You must assign the value TRUE to the property IndexValueVisible in order to use the IndexValueFormat property.

## Signature

```python
obj.IndexValueFormat
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
oMyLabel = oMyShape.Extensions.IsolineLabel
oMyLabel.Visible = True
oMyLabel.IndexValueVisible = True
oMyLabel.IndexValueFormat = "d"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionLength
oMyLabel.Repetition.PercentValue = 30
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndexValueFormat_IRepD3LabelIsolineAdditionalInt.htm`*
