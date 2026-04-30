---
title: "IRepSheetInt.Index"
description: "Returns the index of a worksheet in DIAdem REPORT. The index corresponds with the tab order."
---

# IRepSheetInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for Sheet

Returns the index of a worksheet in DIAdem REPORT. The index corresponds with the tab order.

## Signature

```python
obj.Index
```

## Python example

```python
for oMySheet in dd.Report.Sheets:
    sOutput = sOutput + "Sheet: " + oMySheet.Name + " ; Index: " + oMySheet.Index + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepSheetInt.htm`*
