---
title: "ActiveSheetChanged.OnActiveSheetChanged"
description: "Runs in DIAdem VIEW when the active worksheet changes."
---

# ActiveSheetChanged.OnActiveSheetChanged

!!! abstract "Event &middot; `Scriptview.chm`"
    Event: OnActiveSheetChanged

Runs in DIAdem VIEW when the active worksheet changes.

## Signature

```python
obj.OnActiveSheetChanged
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to one event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td>
</tr>
</table>
</div>

## Python example

```python
dd.AddUserCommandToEvent("View.Events.OnActiveSheetChanged","TransCursor")

def TRANSCURSOR(oNewSheet, oOldSheet):
    oNewSheet.Cursor.Mode = oOldSheet.Cursor.Mode
    oNewSheet.Cursor.Type = oOldSheet.Cursor.Type
    oNewSheet.Cursor.X1 = oOldSheet.Cursor.X1
    oNewSheet.Cursor.Y1 = oOldSheet.Cursor.Y1
    oNewSheet.Cursor.X2 = oOldSheet.Cursor.X2
    oNewSheet.Cursor.Y2 = oOldSheet.Cursor.Y2
    oNewSheet.Cursor.P1 = oOldSheet.Cursor.P1
    oNewSheet.Cursor.P2 = oOldSheet.Cursor.P2
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../properties/itoeventsint-onactivesheetchanged/">OnActiveSheetChanged</a> | <a href="#" data-unresolved="1">Object sOverview</a></p>
</div>
</div>

---

*Source: `Scriptview/events/VIEW_events_ActiveSheetChanged.htm`*
