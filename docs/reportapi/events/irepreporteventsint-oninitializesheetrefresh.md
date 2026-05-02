---
title: "IRepReportEventsInt.OnInitializeSheetRefresh"
description: "Is triggered in DIAdem REPORT before you refresh a worksheet. The event starts the user command that you have assigned to the property Report.Events. OnInitiali"
---

# IRepReportEventsInt.OnInitializeSheetRefresh

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnInitializeSheetRefresh for Events

Is triggered in DIAdem REPORT before you refresh a worksheet. The event starts the user command that you have assigned to the property Report.Events. OnInitializeSheetRefresh . The user command receives a parameter. The parameter receives the Sheet object of the refreshed worksheet. The event applies to all worksheets in a layout. Use the OnInitializeSheetRefresh for SheetEvents property in order to use a separate user command for each worksheet. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnInitializeSheetRefresh
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
AddUserCommandToEvent("dd.Report.Events.OnInitializeSheetRefresh", "MyOnInitializeSheetRefresh")

def MyOnInitializeSheetRefresh(Sheet):
    dd.MsgBox("Sheet: " + Sheet.Name + "\t" + "Number of objects: " + Sheet.Objects.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnInitializeSheetRefresh_IRepReportEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
