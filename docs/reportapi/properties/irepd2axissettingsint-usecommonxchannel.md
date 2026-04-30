---
title: "IRepD2AxisSettingsInt.UseCommonXChannel"
description: "Specifies whether DIAdem REPORT also uses the x-channel of the first curve as the x-channel for all other curves in a 2D axis system."
---

# IRepD2AxisSettingsInt.UseCommonXChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCommonXChannel for 2DAxisSettings

Specifies whether DIAdem REPORT also uses the x-channel of the first curve as the x-channel for all other curves in a 2D axis system.

## Signature

```python
obj.UseCommonXChannel
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve1 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMy2DCurve2 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve2")
oMy2DCurve1.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve2.Shape.YChannel.Reference = "[1]/[3]"
oMy2DAxisSystem.Settings.UseCommonXChannel = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCommonXChannel_IRepD2AxisSettingsInt.htm`*
