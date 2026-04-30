---
title: "IRepReportInt.ResetModified"
description: "Indicates that the current layout in DIAdem REPORT is unchanged."
---

# IRepReportInt.ResetModified

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ResetModified for Report

Indicates that the current layout in DIAdem REPORT is unchanged.

## Signature

```python
obj.ResetModified()
```

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
dd.MsgBoxDisp("Layout modified: " + dd.Report.IsModified)
dd.Report.ResetModified()
dd.MsgBoxDisp("Layout modified: " + dd.Report.IsModified)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ResetModified_IRepReportInt.htm`*
