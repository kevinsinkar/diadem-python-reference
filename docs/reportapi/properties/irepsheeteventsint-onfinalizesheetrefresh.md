---
title: "IRepSheetEventsInt.OnFinalizeSheetRefresh"
description: "Specifies which user command DIAdem REPORT executes after it refreshes a worksheet. The user command receives a parameter. The parameter receives the Sheet obje"
---

# IRepSheetEventsInt.OnFinalizeSheetRefresh

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnFinalizeSheetRefresh for SheetEvents

Specifies which user command DIAdem REPORT executes after it refreshes a worksheet. The user command receives a parameter. The parameter receives the Sheet object of the refreshed worksheet. The property applies only to the specified worksheet. Use the OnFinalizeSheetRefresh for Events property to use the same user command for all worksheets. DIAdem REPORT saves this property with the layout.

## Signature

```python
obj.OnFinalizeSheetRefresh
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.ActiveSheet.Events.OnFinalizeSheetRefresh = "MyOnFinalizeSheetRefresh_perSheet"

def MyOnFinalizeSheetRefresh_perSheet(Sheet):
    dd.MsgBox("Sheet: " + Sheet.Name + "\t" + "Number of objects: " + Sheet.Objects.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnFinalizeSheetRefresh_IRepSheetEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
