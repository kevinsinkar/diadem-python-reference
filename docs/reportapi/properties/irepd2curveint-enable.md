---
title: "IRepD2CurveInt.Enable"
description: "Specifies whether DIAdem REPORT displays the curve in a 2D axis system."
---

# IRepD2CurveInt.Enable

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Enable for 2DCurve

Specifies whether DIAdem REPORT displays the curve in a 2D axis system.

## Signature

```python
obj.Enable
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve1 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "My2DCurve")
oMy2DCurve1.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve2 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "My2DCurve2")
oMy2DCurve2.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve2.Shape.YChannel.Reference = "[1]/[3]"
oMy2DCurve1.Enable = False
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Enable_IRepD2CurveInt.htm`*
