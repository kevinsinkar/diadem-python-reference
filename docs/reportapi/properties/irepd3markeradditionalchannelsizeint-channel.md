---
title: "IRepD3MarkerAdditionalChannelSizeInt.Channel"
description: "Specifies the channel containing the values DIAdem uses for the size of the additional markers of a curve in a 3D axis system in DIAdem REPORT. DIAdem sets the "
---

# IRepD3MarkerAdditionalChannelSizeInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 3DAdditionalMarkerChannelSize

Specifies the channel containing the values DIAdem uses for the size of the additional markers of a curve in a 3D axis system in DIAdem REPORT. DIAdem sets the size of the markers according to the channel values relative to the largest channel value.

## Signature

```python
return_value = obj.Channel
```

## Python example

```python
o3DPoints = dd.Report.ActiveSheet.Objects("My3DAxisSystem").Curves3D(1).Shape
o3DPoints.Settings.Marker.Channel.Reference = "[3]/[1]"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepD3MarkerAdditionalChannelSizeInt.htm`*
