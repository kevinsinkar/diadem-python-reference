---
title: "IRepD2AxisSettingsInt.UseIsometricRatio"
description: "Specifies whether DIAdem REPORT displays both axes of a 2D axis system with the same scale."
---

# IRepD2AxisSettingsInt.UseIsometricRatio

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseIsometricRatio for 2DAxisSettings

Specifies whether DIAdem REPORT displays both axes of a 2D axis system with the same scale.

## Signature

```python
obj.UseIsometricRatio
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
oMy2DAxisSystem.Settings.UseIsometricRatio = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseIsometricRatio_IRepD2AxisSettingsInt.htm`*
