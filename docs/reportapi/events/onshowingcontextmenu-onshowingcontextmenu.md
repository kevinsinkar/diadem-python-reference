---
title: "OnShowingContextMenu.OnShowingContextMenu"
description: "Is triggered in DIAdem REPORT when a context menu displays."
---

# OnShowingContextMenu.OnShowingContextMenu

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnShowingContextMenu

Is triggered in DIAdem REPORT when a context menu displays.

## Signature

```python
obj.OnShowingContextMenu
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to one event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td>
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
<p class="body"><a href="../../properties/irepreporteventsint-onshowingcontextmenu/">OnShowingContextMenu</a> | <a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_events_OnShowingContextMenu.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
