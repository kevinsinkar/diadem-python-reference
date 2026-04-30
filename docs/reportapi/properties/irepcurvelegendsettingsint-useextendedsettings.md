---
title: "IRepCurveLegendSettingsInt.UseExtendedSettings"
description: "Specifies whether DIAdem automatically specifies the best possible display for the legend or whether you can edit all legend settings."
---

# IRepCurveLegendSettingsInt.UseExtendedSettings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseExtendedSettings for CurveLegendSettings

Specifies whether DIAdem automatically specifies the best possible display for the legend or whether you can edit all legend settings.

## Signature

```python
obj.UseExtendedSettings
```

## Python example

```python
oCurveLegendSettings = dd.Report.Sheets(1).Objects("2D-Axis1").CurveLegend.Settings
oCurveLegendSettings.UseExtendedSettings = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseExtendedSettings_IRepCurveLegendSettingsInt.htm`*
