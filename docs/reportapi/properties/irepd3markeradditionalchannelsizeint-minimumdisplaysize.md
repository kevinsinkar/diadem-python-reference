---
title: "IRepD3MarkerAdditionalChannelSizeInt.MinimumDisplaySize"
description: "Specifies the minimum size of the markers at which DIAdem starts drawing additional curve markers in a 3D axis system in DIAdem REPORT."
---

# IRepD3MarkerAdditionalChannelSizeInt.MinimumDisplaySize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MinimumDisplaySize for 3DAdditionalMarkerChannelSize

Specifies the minimum size of the markers at which DIAdem starts drawing additional curve markers in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.MinimumDisplaySize
```

## Python example

```python
o3DPoints = dd.Report.ActiveSheet.Objects("My3DAxisSystem").Curves3D(1).Shape
o3DPoints.Settings.Marker.MinimumDisplaySize = 3
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MinimumDisplaySize_IRepD3MarkerAdditionalChannelSizeInt.htm`*
