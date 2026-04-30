---
title: "IToEventsInt.OnCursorChanged"
description: "Specifies the name of the user command that DIAdem executes when the cursor changes in DIAdem VIEW. This event occurs if you move the cursor, if you change the "
---

# IToEventsInt.OnCursorChanged

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: OnCursorChanged for Events

Specifies the name of the user command that DIAdem executes when the cursor changes in DIAdem VIEW. This event occurs if you move the cursor, if you change the measurement mode or the cursor type, or if you change the active area.

## Signature

```python
obj.OnCursorChanged
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
AddUserCommandToEvent("dd.View.Events.OnCursorChanged","DisplayCursor")

def DisplayCursor(oCursor):
    Text = Text + "Mode : " + oCursor.Mode + vbCrLf
    Text = Text + "Type : " + oCursor.Type + vbCrLf
    Text = Text + "X1   : " + oCursor.X1 + vbCrLf
    Text = Text + "Y1   : " + oCursor.Y1 + vbCrLf
    Text = Text + "X2   : " + oCursor.X2 + vbCrLf
    Text = Text + "Y2   : " + oCursor.Y2 + vbCrLf
    Text = Text + "dX   : " + oCursor.dX + vbCrLf
    Text = Text + "dY   : " + oCursor.dY + vbCrLf
    Text = Text + "P1   : " + oCursor.P1 + vbCrLf
    Text = Text + "P2   : " + oCursor.P2 + vbCrLf
    oCursor.Sheet.Areas(2).DisplayObj.Text = Text
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../events/cursorchanged-oncursorchanged/">OnCursorChanged</a> | <a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_OnCursorChanged_IToEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
