---
title: "IRepCtrlListInt.Copy"
description: "Copies an object in DIAdem REPORT."
---

# IRepCtrlListInt.Copy

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Copy for ReportObjects

Copies an object in DIAdem REPORT.

## Signature

```python
return_value = obj.Copy(NameOrIndex, NewName, InsertOnSheet)
```

## Python example

```python
dd.Report.NewLayout()
oMyObjects = dd.Report.ActiveSheet.Objects
oMyFrame = oMyObjects.Add(dd.eReportObjectFrame,"MyFrame")
oMyCopyFrame = oMyObjects.Copy("MyFrame","MyFrame2",1)
oMyPosition = oMyCopyFrame.Position.ByBorder
oMyPosition.Left = 30
oMyPosition.Bottom = 30
oMyPosition.Height = 40
oMyPosition.Width = 40
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Copy_IRepCtrlListInt.htm`*
