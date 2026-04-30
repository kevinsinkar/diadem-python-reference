---
title: "IRepD2AxisSettingsInt.NSystemsMode"
description: "Specifies whether DIAdem REPORT displays several data channels in one 2D axis system or in several 2D axis systems."
---

# IRepD2AxisSettingsInt.NSystemsMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: NSystemsMode for 2DAxisSettings

Specifies whether DIAdem REPORT displays several data channels in one 2D axis system or in several 2D axis systems.

## Signature

```python
obj.NSystemsMode
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMy2DAxisSystem.Settings.NSystemsMode = dd.e2DAxisNSystems
oMyCurve1 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyFirstCurve")
oMyCurve1.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMyCurve2 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MySecondCurve")
oMyCurve2.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve2.Shape.YChannel.Reference = "[1]/[3]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_NSystemsMode_IRepD2AxisSettingsInt.htm`*
