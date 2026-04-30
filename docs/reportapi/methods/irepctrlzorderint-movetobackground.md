---
title: "IRepCtrlZOrderInt.MoveToBackground"
description: "Moves an object in front of or behind all other objects in a worksheet in DIAdem REPORT."
---

# IRepCtrlZOrderInt.MoveToBackground

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: MoveToBackground for ZOrder

Moves an object in front of or behind all other objects in a worksheet in DIAdem REPORT.

## Signature

```python
obj.MoveToBackground()
```

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorBlue)
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyFrame.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorRed)
oMyFrame.Position.ZOrder.MoveToBackground()
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_MoveToBackground_IRepCtrlZOrderInt.htm`*
