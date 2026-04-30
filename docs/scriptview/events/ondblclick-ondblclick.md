---
title: "OnDblClick.OnDblClick"
description: "Is triggered when an area in double-clicked in DIAdem VIEW."
---

# OnDblClick.OnDblClick

!!! abstract "Event &middot; `Scriptview.chm`"
    Event: OnDblClick

Is triggered when an area in double-clicked in DIAdem VIEW.

## Signature

```python
obj.OnDblClick
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

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
AddUserCommandToEvent("dd.View.Events.OnDblClick", "MyOnDblClick")

def MyOnDblClick(oArea, bProceed):
    dd.MsgBox("DblClick: " + oArea.DisplayObjType)
    bProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../properties/itoeventsint-ondblclick/">OnDblClick</a> | <a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/events/VIEW_events_OnDblClick.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
