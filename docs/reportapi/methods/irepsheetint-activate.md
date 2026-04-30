---
title: "IRepSheetInt.Activate"
description: "Enables the specified worksheet in DIAdem REPORT. The Activate method does not automatically open DIAdem REPORT. The Activate method also works if DIAdem REPORT"
---

# IRepSheetInt.Activate

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Activate for Sheet

Enables the specified worksheet in DIAdem REPORT. The Activate method does not automatically open DIAdem REPORT. The Activate method also works if DIAdem REPORT is not open.

## Signature

```python
obj.Activate()
```

## Python example

```python
dd.WndOpen("REPORT")
for oMySheet in dd.Report.Sheets:
    oMySheet.Activate()
    dd.Pause(2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Activate_IRepSheetInt.htm`*
