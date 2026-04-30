---
title: "IRepSettingsInt.UseAutoScalingNormSeries"
description: "Specifies whether DIAdem REPORT orders the axis ticks in 2D or 3D axis systems as a 1, 2, 5, 10, 20... sequence or as a 2, 2.5, 5, 10, … sequence. When DIAdem s"
---

# IRepSettingsInt.UseAutoScalingNormSeries

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseAutoScalingNormSeries for Settings

Specifies whether DIAdem REPORT orders the axis ticks in 2D or 3D axis systems as a 1, 2, 5, 10, 20... sequence or as a 2, 2.5, 5, 10, … sequence. When DIAdem scales the axes according to standard progression, the range from 0 to 100 is scaled as 20, 40, 60, 80 and 100, otherwise DIAdem scales the axis at 25, 50, 75 and 100.

## Signature

```python
obj.UseAutoScalingNormSeries
```

## Python example

```python
dd.Report.Settings.UseAutoScalingNormSeries = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseAutoScalingNormSeries_IRepSettingsInt.htm`*
