---
title: "IRepD3BoundaryCurveAdditionalInt.AddFullLoadLowerBoundary"
description: "Specifies whether DIAdem REPORT also displays a full load curve when displaying characteristic diagrams in a 3D axis system. To close the full load curve, DIAde"
---

# IRepD3BoundaryCurveAdditionalInt.AddFullLoadLowerBoundary

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AddFullLoadLowerBoundary for 3DAdditionalBoundaryCurve

Specifies whether DIAdem REPORT also displays a full load curve when displaying characteristic diagrams in a 3D axis system. To close the full load curve, DIAdem searches for the smallest and largest x-value of the full load curve. DIAdem connects the points belonging to these two values with a horizontal line at the height of the point with the smaller y-value. DIAdem uses a vertical line to connect the point with the larger y-value with the horizontal line.

## Signature

```python
obj.AddFullLoadLowerBoundary
```

## Python example

```python
o3DAdditionalBoundaryCurve = dd.Report.ActiveSheet.Objects.Item("3DAxis1").Curves3D.Item("3DObj_Curve1").Shape.Extensions.BoundaryCurve
o3DAdditionalBoundaryCurve.Type                      = dd.e3DBoundaryCurveFullLoadCurve
o3DAdditionalBoundaryCurve.AddFullLoadLowerBoundary  = True
o3DAdditionalBoundaryCurve.Visible                   = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AddFullLoadLowerBoundary_IRepD3BoundaryCurveAdditionalInt.htm`*
