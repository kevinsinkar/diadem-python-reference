---
title: "IRepPositionInt.ZOrder"
description: "Specifies the order of an object in DIAdem REPORT."
---

# IRepPositionInt.ZOrder

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ZOrder for ObjectPosition

Specifies the order of an object in DIAdem REPORT.

## Signature

```python
return_value = obj.ZOrder
```

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorBlue)
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyFrame.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorRed)
oMyFrame.Position.ZOrder.Move(-1)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ZOrder_IRepPositionInt.htm`*
