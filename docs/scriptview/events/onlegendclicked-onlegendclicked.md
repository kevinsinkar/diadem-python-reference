---
title: "OnLegendClicked.OnLegendClicked"
description: "Is triggered in DIAdem if you left-click a legend."
---

# OnLegendClicked.OnLegendClicked

!!! abstract "Event &middot; `Scriptview.chm`"
    Event: OnLegendClicked

Is triggered in DIAdem if you left-click a legend.

## Signature

```python
obj.OnLegendClicked
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
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
AddUserCommandToEvent("dd.View.Events.OnLegendClicked", "MyOnLegendClicked")

def MyOnLegendClicked(oArea, oContext):
    dd.MsgBox("Selected curve: " + oContext.CurveIndex)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../properties/itoeventsint-ondblclick/">OnDblClick</a> | <a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/events/VIEW_events_OnLegendClicked.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
