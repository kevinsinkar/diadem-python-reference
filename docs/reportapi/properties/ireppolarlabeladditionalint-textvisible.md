---
title: "IRepPolarLabelAdditionalInt.TextVisible"
description: "Specifies whether DIAdem displays free text to label a curve in a polar axis system in the Line and Points display mode."
---

# IRepPolarLabelAdditionalInt.TextVisible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TextVisible for PolarAdditionalLabel

Specifies whether DIAdem displays free text to label a curve in a polar axis system in the Line and Points display mode.

## Signature

```python
obj.TextVisible
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
oMyLabel.Repetition.Mode = dd.eLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 50
oMyLabel.TextVisible = True
oMyLabel.Text = "*"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TextVisible_IRepPolarLabelAdditionalInt.htm`*
