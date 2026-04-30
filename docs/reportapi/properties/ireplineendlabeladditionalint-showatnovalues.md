---
title: "IRepLineEndLabelAdditionalInt.ShowAtNoValues"
description: "Specifies whether DIAdem REPORT labels each curve section that is between two NoValues."
---

# IRepLineEndLabelAdditionalInt.ShowAtNoValues

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowAtNoValues for AdditionalLineEndLabel

Specifies whether DIAdem REPORT labels each curve section that is between two NoValues.

## Signature

```python
obj.ShowAtNoValues
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Data.GetChannel("[1]/[2]").Values[20] = dd.NoValue
dd.Data.GetChannel("[1]/[2]").Values[200] = dd.NoValue
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyEndLabel = oMyCurve.Shape.Extensions.EndLabel
oMyEndLabel.Position = dd.e2DLineEndLabelPositionLargestXValue
oMyEndLabel.Type = dd.e2DLineEndLabelCustomText
oMyEndLabel.ShowAtNoValues = True
oMyEndLabel.Text = "End"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowAtNoValues_IRepLineEndLabelAdditionalInt.htm`*
