---
title: "IRepPolarMarkerAdditionalInt.MinimumDisplaySize"
description: "Specifies the minimum size of the markers at which DIAdem starts drawing additional curve markers in a polar axis system in DIAdem REPORT."
---

# IRepPolarMarkerAdditionalInt.MinimumDisplaySize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MinimumDisplaySize for PolarAdditionalMarker

Specifies the minimum size of the markers at which DIAdem starts drawing additional curve markers in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.MinimumDisplaySize
```

## Python example

```python
oPolarPoints = dd.Report.ActiveSheet.Objects("MyPolarAxisSystem").CurvesPolar(1).Shape
oPolarPoints.Extensions.Marker.MinimumDisplaySize = 3
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MinimumDisplaySize_IRepPolarMarkerAdditionalInt.htm`*
