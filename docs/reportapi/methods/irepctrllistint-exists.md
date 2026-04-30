---
title: "IRepCtrlListInt.Exists"
description: "Checks whether an object with a specific name exists in DIAdem REPORT."
---

# IRepCtrlListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for ReportObjects

Checks whether an object with a specific name exists in DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
if dd.Report.ActiveSheet.Objects.Exists("MyCircle") :
    dd.MsgBoxDisp("Object already exists.")
else:
    oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
    oMyCircle.Position.ByBorder.Left = 30
    oMyCircle.Position.ByBorder.Bottom = 30
    oMyCircle.Position.ByBorder.Height = 40
    oMyCircle.Position.ByBorder.Width = 40
    oMyCircle.BackgroundColor.SetPredefinedColor(dd.eColorIndexBlue)
    oMyCircle.BorderLine.Color.SetPredefinedColor(dd.eColorIndexRed)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepCtrlListInt.htm`*
