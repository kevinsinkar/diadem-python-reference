---
title: "IRepD3MarkerAdditionalChannelSizeInt.Size"
description: "Specifies the marker sizes in a 3D axis system in DIAdem REPORT."
---

# IRepD3MarkerAdditionalChannelSizeInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for 3DAdditionalMarkerChannelSize

Specifies the marker sizes in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Size
```

## Python example

```python
o3DPoints = dd.Report.ActiveSheet.Objects("My3DAxisSystem").Curves3D(1).Shape
o3DPoints.Settings.Marker.Line.UseCurveColor = False
o3DPoints.Settings.Marker.Line.Color.ColorIndex = dd.eColorIndexBlue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Size_IRepD3MarkerAdditionalChannelSizeInt.htm`*
