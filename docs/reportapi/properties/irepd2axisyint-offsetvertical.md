---
title: "IRepD2AxisYInt.OffsetVertical"
description: "Specifies the vertical displacement of the y-subaxis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYInt.OffsetVertical

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetVertical for 2DAxisY

Specifies the vertical displacement of the y-subaxis in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.OffsetVertical
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
oMyYAxis2 = oMy2DAxisSystem.YAxisList.Add("YAxis2")
oMyYAxis2.OffsetOrigin = dd.e2DAxisOffsetOriginAxisEnd
oMyYAxis2.OffsetHorizontal = 5
oMyYAxis2.OffsetVertical = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetVertical_IRepD2AxisYInt.htm`*
