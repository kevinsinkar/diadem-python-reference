---
title: "IRepD2ShapeObjDifferentialInt"
description: "The 2DDifferential object provides the curve properties of a 2D axis system in the Differential display mode in DIAdem REPORT."
---

# IRepD2ShapeObjDifferentialInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DDifferential

The 2DDifferential object provides the curve properties of a 2D axis system in the Differential display mode in DIAdem REPORT.

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeDifferential, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Type = dd.e2DDifferentialRange
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.BorderLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjdifferentialint-settings/">Settings</a> | <a href="../../properties/irepd2shapeobjdifferentialint-xchannel/">XChannel</a> | <a href="../../properties/irepd2shapeobjdifferentialint-ychannel/">YChannel</a> | <a href="../../properties/irepd2shapeobjdifferentialint-ychanneldifferential/">YChannelDifferential</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2curveint/">2DCurve</a>.<a href="../../properties/irepd2curveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjDifferentialInt.htm`*
