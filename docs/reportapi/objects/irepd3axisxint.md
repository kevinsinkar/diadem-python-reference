---
title: "IRepD3AxisXInt"
description: "The 3DAxisX object provides the properties of the x-axis in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisXInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAxisX

The 3DAxisX object provides the properties of the x-axis in a 3D axis system in DIAdem REPORT.

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
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.DataStructure = dd.e3DDataStructureMatrix
oMyXLabel = oMy3DAxisSystem.AxisList.X.Label
oMyXLabel.Text = "This is the x-axis"
oMyXLabel.Font.Name = "Tahoma"
oMyXLabel.Font.Size = 5
oMyYLabel = oMy3DAxisSystem.AxisList.Y.Label
oMyYLabel.Text = "This is the y-axis"
oMyYLabel.Font.Name = "Tahoma"
oMyYLabel.Font.Size = 5
oMyZLabel = oMy3DAxisSystem.AxisList.Z.Label
oMyZLabel.Text = "This is the z-axis"
oMyZLabel.Font.Name = "Tahoma"
oMyZLabel.Font.Size = 5
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3axisxint-label/">Label</a> | <a href="../../properties/irepd3axisxint-line/">Line</a> | <a href="../../properties/irepd3axisxint-numbers/">Numbers</a> | <a href="../../properties/irepd3axisxint-scaling/">Scaling</a> | <a href="../../properties/irepd3axisxint-targetunit/">TargetUnit</a> | <a href="../../properties/irepd3axisxint-ticktype/">TickType</a> | <a href="../../properties/irepd3axisxint-uselabelautoangle/">UseLabelAutoAngle</a> | <a href="../../properties/irepd3axisxint-usenumbersautoposition/">UseNumbersAutoPosition</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3axislistint/">3DAxisList</a>.<a href="../../properties/irepd3axislistint-x/">X</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3AxisXInt.htm`*
