---
title: "IRepD2MarkerAdditionalInt.MinimumDisplaySize"
description: "Specifies the minimum size of the markers at hich DIAdem starts drawing additional markers of a curve in a 2D axis system in DIAdem REPORT."
---

# IRepD2MarkerAdditionalInt.MinimumDisplaySize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MinimumDisplaySize for 2DAdditionalMarker

Specifies the minimum size of the markers at hich DIAdem starts drawing additional markers of a curve in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.MinimumDisplaySize
```

## Python example

```python
o2DLine = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DLine.Extensions.Marker.MinimumDisplaySize= 3
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MinimumDisplaySize_IRepD2MarkerAdditionalInt.htm`*
