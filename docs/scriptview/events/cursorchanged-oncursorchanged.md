---
title: "CursorChanged.OnCursorChanged"
description: "Triggers when the cursor moves, the measurement mode or the cursor type changes, and when the active area changes, in DIAdem VIEW."
---

# CursorChanged.OnCursorChanged

!!! abstract "Event &middot; `Scriptview.chm`"
    Event: OnCursorChanged

Triggers when the cursor moves, the measurement mode or the cursor type changes, and when the active area changes, in DIAdem VIEW.

## Signature

```python
obj.OnCursorChanged
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
dd.AddUserCommandToEvent("View.Events.OnCursorChanged","DisplayCursor")

def DISPLAYCURSOR(oCursor):
    Text = Text + "Mode : " + oCursor.Mode + "\r\n"
    Text = Text + "Type : " + oCursor.Type + "\r\n"
    Text = Text + "X1   : " + oCursor.X1 + "\r\n"
    Text = Text + "Y1   : " + oCursor.Y1 + "\r\n"
    Text = Text + "X2   : " + oCursor.X2 + "\r\n"
    Text = Text + "Y2   : " + oCursor.Y2 + "\r\n"
    Text = Text + "dX   : " + oCursor.dX + "\r\n"
    Text = Text + "dY   : " + oCursor.dY + "\r\n"
    Text = Text + "P1   : " + oCursor.P1 + "\r\n"
    Text = Text + "P2   : " + oCursor.P2 + "\r\n"
    oCursor.Sheet.Areas(2).DisplayObj.Text = Text
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"> <a href="../../properties/itoeventsint-oncursorchanged/">OnCursorChanged</a> | <a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/events/VIEW_events_CursorChanged.htm`*
