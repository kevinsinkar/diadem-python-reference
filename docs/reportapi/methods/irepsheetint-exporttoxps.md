---
title: "IRepSheetInt.ExportToXPS"
description: "Exports a worksheet from DIAdem REPORT to an XPS file (XML paper specification)."
---

# IRepSheetInt.ExportToXPS

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ExportToXPS for Sheet

Exports a worksheet from DIAdem REPORT to an XPS file (XML paper specification).

## Signature

```python
obj.ExportToXPS(FileName)
```

## Python example

```python
dd.Report.NewLayout()
oMySheet = dd.Report.Sheets.Add("NewSheet")
oMyCircle = oMySheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.BackgroundColor.SetPredefinedColor(dd.eColorIndexGreen)
oMyCircle.BorderLine.Width = dd.eLineWidth0200
oMyCircle.BorderLine.LineType = dd.eLineTypeSolid
oMyCircle.BorderLine.Color.SetPredefinedColor(dd.eColorIndexRed)
oMySheet.ExportToXPS("d:\\MySheet")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ExportToXPS_IRepSheetInt.htm`*
