---
title: "IRepBoxWhiskerLineInt.Interval"
description: "Specifies the line intervals of broken lines in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerLineInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for 2DBoxWhiskerLine

Specifies the line intervals of broken lines in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
obj.Interval
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.WhiskerLine.LineType = dd.eLineTypeDashDot
o2DBoxWhisker.Settings.WhiskerLine.Interval = 1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepBoxWhiskerLineInt.htm`*
