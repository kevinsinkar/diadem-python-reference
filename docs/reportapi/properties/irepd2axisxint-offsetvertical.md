---
title: "IRepD2AxisXInt.OffsetVertical"
description: "Specifies the vertical displacement of the x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXInt.OffsetVertical

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetVertical for 2DAxisX

Specifies the vertical displacement of the x-axis in a 2D axis system in DIAdem REPORT.

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
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMy2DAxisSystem.XAxis.OffsetOrigin = dd.e2DAxisOffsetOriginAxisBegin
oMy2DAxisSystem.XAxis.OffsetVertical = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetVertical_IRepD2AxisXInt.htm`*
