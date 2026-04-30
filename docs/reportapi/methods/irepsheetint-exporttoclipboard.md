---
title: "IRepSheetInt.ExportToClipboard"
description: "Exports a DIAdem REPORT worksheet as a graphic to the Windows clipboard."
---

# IRepSheetInt.ExportToClipboard

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ExportToClipboard for Sheet

Exports a DIAdem REPORT worksheet as a graphic to the Windows clipboard.

## Signature

```python
obj.ExportToClipboard()
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
oMySheet.ExportToClipboard()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ExportToClipboard_IRepSheetInt.htm`*
