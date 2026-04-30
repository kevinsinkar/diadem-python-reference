---
title: "IRepSheetInt.Objects"
description: "Specifies the objects in a DIAdem REPORT worksheet."
---

# IRepSheetInt.Objects

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Objects for Sheet

Specifies the objects in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Objects
```

## Python example

```python
for oMySheet in dd.Report.Sheets:
    dd.MsgBoxDisp(oMySheet.Objects.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Objects_IRepSheetInt.htm`*
