---
title: "IToEventsInt.OnShowingContextMenu"
description: "Specifies the name of the user command that DIAdem executes when you open a context menu in DIAdem VIEW."
---

# IToEventsInt.OnShowingContextMenu

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: OnShowingContextMenu for Events

Specifies the name of the user command that DIAdem executes when you open a context menu in DIAdem VIEW.

## Signature

```python
obj.OnShowingContextMenu
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
dd.AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu", "MyOnShowingContextMenu")
dd.AddUserCommandToEvent("dd.View.Events.OnContextMenuPointSelected","MyOnContextMenuPointSelected")

def MyOnShowingContextMenu(oArea, oMenuPoints):
    oMenuPoints.RemoveAll
    oMenuPoints.Add("MyMenuPoint1", 1)
    oMenuPoints.Add("MyMenuPoint2", 2)

def MyOnContextMenuPointSelected(oArea, oMenuPoint):
    pass
    # select oMenuPoint.ID
    # case 1    MsgBoxDisp("MyMenuPoint1 selected")
    # case 2    MsgBoxDisp("MyMenuPoint2 selected")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="../../events/onshowingcontextmenu-onshowingcontextmenu/">OnShowingContextMenu</a> | <a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_OnShowingContextMenu_IToEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
