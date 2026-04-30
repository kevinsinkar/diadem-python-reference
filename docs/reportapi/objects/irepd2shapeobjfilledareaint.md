---
title: "IRepD2ShapeObjFilledAreaInt"
description: "The 2DFilledArea object provides the curve properties of a 2D axis system in the Filled Area display mode in DIAdem REPORT."
---

# IRepD2ShapeObjFilledAreaInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DFilledArea

The 2DFilledArea object provides the curve properties of a 2D axis system in the Filled Area display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeFilledArea, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
oMySettings.FillEffects.Pattern = dd.eFillPatternFilled
oMySettings.FillEffects.Color.SetPredefinedColor(dd.eColorIndexRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjfilledareaint-settings/">Settings</a> | <a href="../../properties/irepd2shapeobjfilledareaint-xchannel/">XChannel</a> | <a href="../../properties/irepd2shapeobjfilledareaint-ychannel/">YChannel</a> | <a href="../../properties/irepd2shapeobjfilledareaint-ychanneldifferential/">YChannelDifferential</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjFilledAreaInt.htm`*
