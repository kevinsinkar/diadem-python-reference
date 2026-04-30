---
title: "IRepD2AxisYInt.OffsetOrigin"
description: "Specifies the reference point to which the displacement of the y-axis in a 2D axis system in DIAdem REPORT refers."
---

# IRepD2AxisYInt.OffsetOrigin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetOrigin for 2DAxisY

Specifies the reference point to which the displacement of the y-axis in a 2D axis system in DIAdem REPORT refers.

## Signature

```python
obj.OffsetOrigin
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.Y1 = 20
oMyPos.X2 = 80
oMyPos.Y2 = 80
oMy2DAxisSystem.YAxis.OffsetOrigin = dd.e2DAxisOffsetOriginAxisBegin
oMy2DAxisSystem.YAxis.OffsetHorizontal = 10
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetOrigin_IRepD2AxisYInt.htm`*
