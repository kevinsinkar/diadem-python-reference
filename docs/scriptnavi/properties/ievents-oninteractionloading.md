---
title: "IEvents.OnInteractionLoading"
description: "Specifies the name of the user command that DIAdem executes before executing a command which was called when data was dragged and dropped into the Data Portal."
---

# IEvents.OnInteractionLoading

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: OnInteractionLoading for Events <Navigator>

Specifies the name of the user command that DIAdem executes before executing a command which was called when data was dragged and dropped into the Data Portal.

## Signature

```python
obj.OnInteractionLoading
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to one event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
AddUserCommandToEvent("dd.Navigator.Events.OnInteractionLoading","MyInteractionLoading")
AddUserCommandToEvent("dd.Navigator.Events.OnInteractionLoaded","MyInteractionLoaded")

def MyInteractionLoading():
    # select MsgBoxDisp("Delete dd.Data Portal before loading new data?","MB_YESNO",,2)
    # case "IDYes"
    dd.Data.Root.Clear
    # case "IDNo"
    MsgBoxDisp("New data will be appended to existing data." + VBCrLf, "MB_NOBUTTON", "MsgTypeNoteNoIcon",, 3, TRUE)
    # case "IDCancel"
    MsgBoxDisp("Cancelled by user", "MB_NOBUTTON", "MsgTypeWarning",, 3)

def MyInteractionLoaded():
    MsgBoxDisp("Open dd.Report Wizard")
    WndOpen ("REPORT")
    WizardStart("WizChart","","PORTAL")
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="../../events/oninteractionloaded-oninteractionloaded/">Event: OnInteractionLoaded</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_OnInteractionLoading_IEvents.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
