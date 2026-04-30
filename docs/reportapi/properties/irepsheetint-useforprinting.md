---
title: "IRepSheetInt.UseForPrinting"
description: "Specifies that DIAdem includes a worksheet when printing. Use the SetUseForPrinting for Sheets method to specify whether DIAdem includes all worksheets when pri"
---

# IRepSheetInt.UseForPrinting

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseForPrinting for Sheet

Specifies that DIAdem includes a worksheet when printing. Use the SetUseForPrinting for Sheets method to specify whether DIAdem includes all worksheets when printing.

## Signature

```python
obj.UseForPrinting
```

## Python example

```python
for oMySheet in dd.Report.Sheets:
    oMySheet.UseForPrinting = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseForPrinting_IRepSheetInt.htm`*
