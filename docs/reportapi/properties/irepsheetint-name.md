---
title: "IRepSheetInt.Name"
description: "Specifies the name of a worksheet in DIAdem REPORT."
---

# IRepSheetInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for Sheet

Specifies the name of a worksheet in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
dd.Report.Sheets.Add("NewSheet")
oMySheets = dd.Report.Sheets
for oSheet in oMySheets:
    dd.MsgBoxDisp("Index: " + oSheet.Index + "\r\n" + "Name: " + oSheet.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepSheetInt.htm`*
