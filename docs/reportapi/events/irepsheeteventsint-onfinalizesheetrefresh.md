---
title: "IRepSheetEventsInt.OnFinalizeSheetRefresh"
description: "Is triggered in DIAdem REPORT after you refresh a worksheet. The event starts the user command that you have assigned to the property Report.Events. OnFinalizeS"
---

# IRepSheetEventsInt.OnFinalizeSheetRefresh

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnFinalizeSheetRefresh for SheetEvents

Is triggered in DIAdem REPORT after you refresh a worksheet. The event starts the user command that you have assigned to the property Report.Events. OnFinalizeSheetRefresh . The user command receives a parameter. The parameter receives the Sheet object of the refreshed worksheet. The event applies only to the specified worksheet. Use the OnFinalizeSheetRefresh for Events event to use the same user command for all worksheets. Refer to Working with Events in DIAdem for further information on events in DIAdem.

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
AddUserCommandToEvent("dd.Report.ActiveSheet.Events.OnFinalizeSheetRefresh", "MyOnFinalizeSheetRefresh_perSheet")

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

*Source: `ReportApi/events/Report_event_OnFinalizeSheetRefresh_IRepSheetEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
