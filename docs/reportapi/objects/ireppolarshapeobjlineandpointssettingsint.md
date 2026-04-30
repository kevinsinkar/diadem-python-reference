---
title: "IRepPolarShapeObjLineAndPointsSettingsInt"
description: "The PolarLineAndPointsSettings object provides the properties of a polar curve in the display type Line and Points in DIAdem REPORT."
---

# IRepPolarShapeObjLineAndPointsSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarLineAndPointsSettings

The PolarLineAndPointsSettings object provides the properties of a polar curve in the display type Line and Points in DIAdem REPORT.

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
oMyLine = oMyCurve.Shape.Settings.Line
oMyLine.LineType = dd.eLineTypeSolid
oMyLine.Color.ColorIndex = dd.eColorIndexBlue
oMyLine.Width = dd.eLineWidth0050
oMyLine.ConnectNoValueNeighbors = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarshapeobjlineandpointssettingsint-line/">Line</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarshapeobjlineandpointsint/">PolarLineAndPoints</a>.<a href="../../properties/ireppolarshapeobjlineandpointsint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarShapeObjLineAndPointsSettingsInt.htm`*
