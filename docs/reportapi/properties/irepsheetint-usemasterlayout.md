---
title: "IRepSheetInt.UseMasterLayout"
description: "Specifies whether the current worksheet in DIAdem REPORT is connected to a master layout. Use the Connect method to assign a master layout to a layout."
---

# IRepSheetInt.UseMasterLayout

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseMasterLayout for Sheet

Specifies whether the current worksheet in DIAdem REPORT is connected to a master layout. Use the Connect method to assign a master layout to a layout.

## Signature

```python
obj.UseMasterLayout
```

## Python example

```python
for oMySheet in dd.Report.Sheets:
    dd.MsgBoxDisp(oMySheet.UseMasterLayout)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseMasterLayout_IRepSheetInt.htm`*
