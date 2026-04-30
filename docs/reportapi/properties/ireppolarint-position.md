---
title: "IRepPolarInt.Position"
description: "Specifies the position of a polar axis system in a DIAdem REPORT worksheet."
---

# IRepPolarInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for PolarSystem

Specifies the position of a polar axis system in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
```

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPolarAxisSystem.Position.ByCoordinate.X1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.Y1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.X2 = 60
oMyPolarAxisSystem.Position.ByCoordinate.Y2 = 60
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepPolarInt.htm`*
