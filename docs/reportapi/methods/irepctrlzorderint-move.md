---
title: "IRepCtrlZOrderInt.Move"
description: "Moves an object in front of or behind the other objects in a worksheet in DIAdem REPORT."
---

# IRepCtrlZOrderInt.Move

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Move for ZOrder

Moves an object in front of or behind the other objects in a worksheet in DIAdem REPORT.

## Signature

```python
obj.Move(ZOrderDelta)
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

*Source: `ReportApi/methods/Report_method_Move_IRepCtrlZOrderInt.htm`*
