---
title: "IRepD3MarkerAdditionalChannelSizeInt.Filling"
description: "Specifies the properties of the curve marker filling in a 3D axis system in DIAdem REPORT."
---

# IRepD3MarkerAdditionalChannelSizeInt.Filling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Filling for 3DAdditionalMarkerChannelSize

Specifies the properties of the curve marker filling in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Filling
```

## Python example

```python
o3DPoints = dd.Report.ActiveSheet.Objects("My3DAxisSystem").Curves3D(1).Shape
o3DPoints.Settings.Marker.Filling.UseCurveColor = False
o3DPoints.Settings.Marker.Filling.ColorIndex = dd.eColorIndexBlue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Filling_IRepD3MarkerAdditionalChannelSizeInt.htm`*
