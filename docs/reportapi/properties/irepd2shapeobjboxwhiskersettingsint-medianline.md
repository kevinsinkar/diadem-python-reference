---
title: "IRepD2ShapeObjBoxWhiskerSettingsInt.MedianLine"
description: "Specifies the line property of the median lines in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerSettingsInt.MedianLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MedianLine for 2DBoxWhiskerSettings

Specifies the line property of the median lines in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.MedianLine
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.MedianLine.Width = dd.eLineWidth0070
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MedianLine_IRepD2ShapeObjBoxWhiskerSettingsInt.htm`*
