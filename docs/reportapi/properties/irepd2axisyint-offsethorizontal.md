---
title: "IRepD2AxisYInt.OffsetHorizontal"
description: "Specifies the horizontal displacement of the y-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYInt.OffsetHorizontal

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetHorizontal for 2DAxisY

Specifies the horizontal displacement of the y-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.OffsetHorizontal
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMy2DAxisSystem.YAxis.OffsetOrigin = dd.e2DAxisOffsetOriginAxisBegin
oMy2DAxisSystem.YAxis.OffsetHorizontal = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetHorizontal_IRepD2AxisYInt.htm`*
