---
title: "IToEventsInt"
description: "The Events object provides the user commands assigned to an event in DIAdem VIEW. DIAdem saves the Events object in the VIEW layout file."
---

# IToEventsInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Events

The Events object provides the user commands assigned to an event in DIAdem VIEW. DIAdem saves the Events object in the VIEW layout file.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to one event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def MyOnShowingContextMenu(oArea, oMenuPoints):
    oMenuPoints.RemoveAll
    oMenuPoints.Add("MyMenuPoint1", 1)
    oMenuPoints.Add("MyMenuPoint2", 2)

def MyOnContextMenuPointSelected(oArea, oMenuPoint):
    # select oMenuPoint.ID
    # case 1
    MsgBoxDisp("MyMenuPoint1 selected")
    # case 2
    MsgBoxDisp("MyMenuPoint2 selected")

AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu", "MyOnShowingContextMenu")
AddUserCommandToEvent("dd.View.Events.OnContextMenuPointSelected","MyOnContextMenuPointSelected")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoeventsint-onactivesheetchanged/">OnActiveSheetChanged</a> | <a href="../../properties/itoeventsint-oncontextmenupointselected/">OnContextMenuPointSelected</a> | <a href="../../properties/itoeventsint-oncursorchanged/">OnCursorChanged</a> | <a href="../../properties/itoeventsint-ondblclick/">OnDblClick</a> | <a href="../../properties/itoeventsint-ondrop/">OnDrop</a> | <a href="../../properties/itoeventsint-ondropallowed/">OnDropAllowed</a> | <a href="../../properties/itoeventsint-onlayoutloaded/">OnLayoutLoaded</a> | <a href="../../properties/itoeventsint-onlegendclicked/">OnLegendClicked</a> | <a href="../../properties/itoeventsint-onshowingcontextmenu/">OnShowingContextMenu</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../view/">View</a>.<a href="../../properties/view-events/">Events</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
