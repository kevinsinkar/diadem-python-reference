---
title: "IRepSheetInt.TagStored"
description: "Specifies a tag for a worksheet in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in"
---

# IRepSheetInt.TagStored

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TagStored for Sheet

Specifies a tag for a worksheet in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in a program, for example, for special treatment of the object. The tag does not affect the behavior of the worksheet. DIAdem saves this tag with the layout.

## Signature

```python
obj.TagStored
```

## Python example

```python
oMyReportSheet = dd.Report.ActiveSheet
oMyReportSheet.TagStored = "Active sheet"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TagStored_IRepSheetInt.htm`*
