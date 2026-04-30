---
title: "IRepD2ShapeObjBoxWhiskerInt.YChannels"
description: "Specifies the y-channel of a curve in a 2D axis system in the Box-Whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerInt.YChannels

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YChannels for 2DBoxWhisker

Specifies the y-channel of a curve in a 2D axis system in the Box-Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.YChannels
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.XChannel.Reference = ""
o2DBoxWhisker.YChannels.RemoveAll()
o2DBoxWhisker.YChannels.Add("[1]/[1]")
o2DBoxWhisker.YChannels.Add("[1]/[2]")
o2DBoxWhisker.YChannels.Add("[1]/[3]")
o2DBoxWhisker.YChannels.Add("[1]/[4]")
o2DBoxWhisker.YChannels.Add("[1]/[5]")
o2DBoxWhisker.YChannels.Add("[1]/[5]")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YChannels_IRepD2ShapeObjBoxWhiskerInt.htm`*
