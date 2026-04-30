---
title: "OnLayoutLoaded.OnLayoutLoaded"
description: "Is triggered in DIAdem VIEW after a layout is loaded."
---

# OnLayoutLoaded.OnLayoutLoaded

!!! abstract "Event &middot; `Scriptview.chm`"
    Event: OnLayoutLoaded

Is triggered in DIAdem VIEW after a layout is loaded.

## Signature

```python
obj.OnLayoutLoaded
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the VBS example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to an event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td>
</tr>
</table>
</div>

## Python example

```python
dd.AddUserCommandToEvent("View.Events.OnLayoutLoaded", "ON_VIEW_LAYOUT_LOADED_EVENT")

def ON_VIEW_LAYOUT_LOADED_EVENT():

    for sheetNo in range( 1, dd.View.Sheets.Count+1):
        dd.View.Sheets(sheetNo).Name = "Page_" + dd.str(sheetNo)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/events/VIEW_events_OnLayoutLoaded.htm`*
