---
title: "IRepReportInt.Events"
description: "Returns the object in DIAdem REPORT that provides the events in DIAdem REPORT."
---

# IRepReportInt.Events

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Events for Report

Returns the object in DIAdem REPORT that provides the events in DIAdem REPORT.

## Signature

```python
return_value = obj.Events
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.AddUserCommandToEvent("dd.Report.Events.OnFinalizeSheetRefresh","MyOnFinalizeSheetRefresh")

def MyOnFinalizeSheetRefresh(Sheet):
    MsgBoxDisp("Refresh completed")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Events_IRepReportInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
