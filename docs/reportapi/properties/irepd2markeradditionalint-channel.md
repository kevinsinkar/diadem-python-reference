---
title: "IRepD2MarkerAdditionalInt.Channel"
description: "Specifies the channel containing the values DIAdem uses for the size of the additional markers of a curve in a 2D axis system in DIAdem REPORT. DIAdem sets the "
---

# IRepD2MarkerAdditionalInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 2DAdditionalMarker

Specifies the channel containing the values DIAdem uses for the size of the additional markers of a curve in a 2D axis system in DIAdem REPORT. DIAdem sets the size of the markers according to the channel values relative to the largest channel value.

## Signature

```python
return_value = obj.Channel
```

## Python example

```python
o2DLine = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DLine.Extensions.Marker.Channel.Reference = "[3]/[1]"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepD2MarkerAdditionalInt.htm`*
