---
title: "IRepCtrlZOrderInt.MoveToForeground"
description: "Moves an object in front of all other objects in a worksheet in DIAdem REPORT."
---

# IRepCtrlZOrderInt.MoveToForeground

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: MoveToForeground for ZOrder

Moves an object in front of all other objects in a worksheet in DIAdem REPORT.

## Signature

```python
obj.MoveToForeground()
```

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorBlue)
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyFrame.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorRed)
oMyCircle.Position.ZOrder.MoveToForeground()
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_MoveToForeground_IRepCtrlZOrderInt.htm`*
