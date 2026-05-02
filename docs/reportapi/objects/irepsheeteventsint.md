---
title: "IRepSheetEventsInt"
description: "The SheetEvents object provides the events of a worksheet in DIAdem REPORT. Note Refer to Working with Events in DIAdem for further information."
---

# IRepSheetEventsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SheetEvents

The SheetEvents object provides the events of a worksheet in DIAdem REPORT. Note Refer to Working with Events in DIAdem for further information.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Refer to <a href="#" data-unresolved="1">Working with Events in DIAdem</a> for further information.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.AddUserCommandToEvent("dd.Report.Events.OnFinalizeSheetRefresh","MyFinalizeRefresh")

def MyFinalizeRefresh():
    MsgBoxDisp("Refresh of sheet completed: " + dd.Report.ActiveSheet.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsheeteventsint-onfinalizesheetrefresh/">OnFinalizeSheetRefresh</a> | <a href="../../properties/irepsheeteventsint-oninitializesheetrefresh/">OnInitializeSheetRefresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsheetint/">Sheet</a>.<a href="../../properties/irepsheetint-events/">Events</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSheetEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
