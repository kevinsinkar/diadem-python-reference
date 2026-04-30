---
title: "IRepD3LabelRepetitionInt"
description: "The 3DLabelRepetition object provides the properties of the label repetitions in a 3D display in DIAdem REPORT."
---

# IRepD3LabelRepetitionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DLabelRepetition

The 3DLabelRepetition object provides the properties of the label repetitions in a 3D display in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3labelrepetitionint-mode/">Mode</a> | <a href="../../properties/irepd3labelrepetitionint-nvalue/">NValue</a> | <a href="../../properties/irepd3labelrepetitionint-percentvalue/">PercentValue</a> | <a href="../../properties/irepd3labelrepetitionint-showatbegin/">ShowAtBegin</a> | <a href="../../properties/irepd3labelrepetitionint-showatend/">ShowAtEnd</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3labelisolineadditionalint/">3DAdditionalIsolineLabel</a>.<a href="../../properties/irepd3labelisolineadditionalint-repetition/">Repetition</a> | <a href="../irepd3labeladditionalint/">3DAdditionalLabel</a>.<a href="../../properties/irepd3labeladditionalint-repetition/">Repetition</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3LabelRepetitionInt.htm`*
