---
title: "IRepD2CurveListInt.DefaultShapeType"
description: "Specifies the default display type for new curves in a 2D axis system in DIAdem REPORT. You can use the ChangeShape for 2DCurves method to change the display mo"
---

# IRepD2CurveListInt.DefaultShapeType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DefaultShapeType for 2DCurves

Specifies the default display type for new curves in a 2D axis system in DIAdem REPORT. You can use the ChangeShape for 2DCurves method to change the display mode.

## Signature

```python
obj.DefaultShapeType
```

## Python example

```python
dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem").Curves2D.DefaultShapeType = dd.e2DShapeBars
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DefaultShapeType_IRepD2CurveListInt.htm`*
