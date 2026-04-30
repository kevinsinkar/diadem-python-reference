---
title: "IRepD3InterpolationInt.DataReductionMode"
description: "Specifies in the data reduction of the display points of a 3D axis system in the display modes Surface or Characteristic diagram whether DIAdem displays the gre"
---

# IRepD3InterpolationInt.DataReductionMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DataReductionMode for 3DInterpolation

Specifies in the data reduction of the display points of a 3D axis system in the display modes Surface or Characteristic diagram whether DIAdem displays the greatest or the smallest point of a grid cell.

## Signature

```python
obj.DataReductionMode
```

## Python example

```python
oMyReportObj = D3AxisSystemDropContext.AxisSystem.Curves3D.Add.Shape.Settings.Interpolation
dd.MsgBoxDisp(oMyReportObj.DataReductionMode)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DataReductionMode_IRepD3InterpolationInt.htm`*
