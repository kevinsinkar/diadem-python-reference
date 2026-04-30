---
title: "IRepD3InterpolationInt.DataReductionResolution"
description: "Specifies the grid resolution in the data reduction of the display points of a 3D axis system in the display modes Surface or Characteristic diagram . The coars"
---

# IRepD3InterpolationInt.DataReductionResolution

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DataReductionResolution for 3DInterpolation

Specifies the grid resolution in the data reduction of the display points of a 3D axis system in the display modes Surface or Characteristic diagram . The coarser the grid, the faster the display. In many cases the differences between the different resolutions are hardly visible. DIAdem only includes the property DataReductionResolution if you assigned the value e3DDataReductionTypeGrid to the DataReductionType property .

## Signature

```python
obj.DataReductionResolution
```

## Python example

```python
oMyReportObj = D3AxisSystemDropContext.AxisSystem.Curves3D.Add.Shape.Settings.Interpolation
dd.MsgBoxDisp(oMyReportObj.DataReductionResolution)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DataReductionResolution_IRepD3InterpolationInt.htm`*
