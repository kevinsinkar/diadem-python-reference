---
title: "OnDrop.OnDrop"
description: "Is triggered in DIAdem VIEW when you drag and drop elements such as one or several channels, a channel group, or one or more properties from the Data Portal int"
---

# OnDrop.OnDrop

!!! abstract "Event &middot; `Scriptview.chm`"
    Event: OnDrop

Is triggered in DIAdem VIEW when you drag and drop elements such as one or several channels, a channel group, or one or more properties from the Data Portal into an area. The area must be a Channel Table , 2D-Axis System , Bode , Polar , Orbit , Shaft Centerline , Contour , Graphics , Video , or a Textbox display type. The event is not triggered for the display types Map and Dialog Box . The event can only trigger if you can Drop data. The event is triggered if the cursor is above an area in DIAdem VIEW and you release the left mouse button.

## Signature

```python
obj.OnDrop
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
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to an event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
AddUserCommandToEvent("dd.View.Events.OnDropAllowed", "MyOnDropAllowed")
AddUserCommandToEvent("dd.View.Events.OnDrop", "MyOnDrop")

def MyOnDropAllowed(oContext, oDropInformation, ByRef DropEffect):
    oMyElem = oDropInformation.DiademElements
    DropEffect = eDropEffectNone
    if oMyElem.Count = 1:
        if oMyElem(1).IsKindOf(eDataChannel):
            if oMyElem(1).DataType = DataTypeFloat64:
                DropEffect = eDropEffectCopy

def MyOnDrop(oContext, oDropInformation, ByRef bProceed):
    MsgBoxDisp(oDropInformation.DIAdemElements(1).Name + " / " + oDropInformation.DIAdemElements(1).Size)
    bProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../properties/itoeventsint-ondblclick/">OnDblClick</a> | <a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/events/VIEW_events_OnDrop.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
