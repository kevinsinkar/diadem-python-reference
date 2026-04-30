---
title: "IRepD2ShapeObjBoxWhiskerSettingsInt.WhiskerMode"
description: "Specifies the limit values of the whiskers in a 2D axis system in the box whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerSettingsInt.WhiskerMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: WhiskerMode for 2DBoxWhiskerSettings

Specifies the limit values of the whiskers in a 2D axis system in the box whisker display mode in DIAdem REPORT.

## Signature

```python
obj.WhiskerMode
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.WhiskerMode = dd.e2DWhiskerModeMinMax
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_WhiskerMode_IRepD2ShapeObjBoxWhiskerSettingsInt.htm`*
