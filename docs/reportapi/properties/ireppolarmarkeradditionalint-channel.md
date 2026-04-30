---
title: "IRepPolarMarkerAdditionalInt.Channel"
description: "Specifies the channel containing the values DIAdem uses for the size of the additional markers of a curve in a polar axis system in DIAdem REPORT. DIAdem sets t"
---

# IRepPolarMarkerAdditionalInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for PolarAdditionalMarker

Specifies the channel containing the values DIAdem uses for the size of the additional markers of a curve in a polar axis system in DIAdem REPORT. DIAdem sets the size of the markers according to the channel values relative to the largest channel value.

## Signature

```python
return_value = obj.Channel
```

## Python example

```python
oPolarLineAndPoints = dd.Report.ActiveSheet.Objects.Item("2DPolar1").CurvesPolar.Item("2DPolar1_Curve1").Shape
oPolarLineAndPoints.Extensions.Marker.Channel.Reference = "[1]/[1]"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepPolarMarkerAdditionalInt.htm`*
