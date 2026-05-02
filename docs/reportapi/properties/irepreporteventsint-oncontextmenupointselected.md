---
title: "IRepReportEventsInt.OnContextMenuPointSelected"
description: "Is triggered when an item in a context menu is selected in DIAdem REPORT."
---

# IRepReportEventsInt.OnContextMenuPointSelected

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnContextMenuPointSelected for Events

Is triggered when an item in a context menu is selected in DIAdem REPORT.

## Signature

```python
obj.OnContextMenuPointSelected
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.AddUserCommandToEvent("dd.Report.Events.OnShowingContextMenu", "MyOnShowingContextMenu")
dd.AddUserCommandToEvent("dd.Report.Events.OnContextMenuPointSelected","MyOnContextMenuPointSelected")

def MyOnShowingContextMenu(oMenuPoints):
    if dd.Report.SelectedObjects.Count > 0:
        sObject = dd.Report.SelectedObjects(1).Name
        oMenuPoints.Add(sObject + ": MyMenuPoint1", 1)
        oMenuPoints.Add(sObject + ": MyMenuPoint2", 2)

def MyOnContextMenuPointSelected(oMenuPoint):
    if dd.Report.SelectedObjects.Count > 0:
        sObject = dd.Report.SelectedObjects(1).Name
    # select oMenuPoint.ID
    # case 1    MsgBoxDisp(sObject + ": MyMenuPoint1 selected")
    # case 2    MsgBoxDisp(sObject + ": MyMenuPoint2 selected")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnContextMenuPointSelected_IRepReportEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
