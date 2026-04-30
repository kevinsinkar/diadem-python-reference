---
title: "IRepBoxWhiskerLineInt.UseBorderColor"
description: "Specifies whether DIAdem REPORT also uses the line color of the box for the whisker, in a 2D axis system in the Box Whisker display mode."
---

# IRepBoxWhiskerLineInt.UseBorderColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseBorderColor for 2DBoxWhiskerLine

Specifies whether DIAdem REPORT also uses the line color of the box for the whisker, in a 2D axis system in the Box Whisker display mode.

## Signature

```python
obj.UseBorderColor
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.WhiskerLine.Color.ColorIndex = dd.eColorIndexBlue
o2DBoxWhisker.Settings.WhiskerLine.UseBorderColor = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseBorderColor_IRepBoxWhiskerLineInt.htm`*
