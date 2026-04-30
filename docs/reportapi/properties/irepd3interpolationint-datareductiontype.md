---
title: "IRepD3InterpolationInt.DataReductionType"
description: "Specifies whether and how DIAdem performs a data reduction of the display points of a 3D axis system in the display type Area or Map in DIAdem-REPORT. The data "
---

# IRepD3InterpolationInt.DataReductionType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DataReductionType for 3DInterpolation

Specifies whether and how DIAdem performs a data reduction of the display points of a 3D axis system in the display type Area or Map in DIAdem-REPORT. The data reduction enables DIAdem to display the triple data much faster. In many cases, the data reduction only marginally changes the display.

## Signature

```python
obj.DataReductionType
```

## Python example

```python
oMyReportObj = D3AxisSystemDropContext.AxisSystem.Curves3D.Add.Shape.Settings.Interpolation
dd.MsgBoxDisp(oMyReportObj.DataReductionType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DataReductionType_IRepD3InterpolationInt.htm`*
