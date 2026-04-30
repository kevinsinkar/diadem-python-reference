---
title: "IRepD2AxisXInt.TickDisplay"
description: "Specifies the tick properties of the x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXInt.TickDisplay

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TickDisplay for 2DAxisX

Specifies the tick properties of the x-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.TickDisplay
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyTickDisplay = oMy2DAxisSystem.XAxis.TickDisplay
oMyTickDisplay.UseAutoSize = False
oMyTickDisplay.Size = 2
oMyTickDisplay.Type = dd.e2DAxisXTickTop
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TickDisplay_IRepD2AxisXInt.htm`*
