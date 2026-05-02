---
title: "TabPageCtrl.EventMouseDown"
description: "Triggers in user dialog boxes when a tab of the TabPageCtrl control is clicked or right-clicked."
---

# TabPageCtrl.EventMouseDown

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventMouseDown for TabPageCtrl

Triggers in user dialog boxes when a tab of the TabPageCtrl control is clicked or right-clicked.

## Signature

```python
dd.EventMouseDown(ByRef This, Index, Button, Shift, X, Y)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def TabPageCtrl1_EventMouseDown(This, Index, Button, Shift, X, Y):
    MsgBoxDisp("Mouse button pressed at X="& X &" Y="&Y &", "&This.Pages(Index).Title)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../methods/tosudviewobint-mapxdlutopixel/">MapXDluToPixel</a> | <a href="../../methods/tosudviewobint-mapxpixeltodlu/">MapXPixelToDlu</a> | <a href="../../methods/tosudviewobint-mapydlutopixel/">MapYDluToPixel</a> | <a href="../../methods/tosudviewobint-mapypixeltodlu/">MapYPixelToDlu</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventMouseDown_TabPageCtrl.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
