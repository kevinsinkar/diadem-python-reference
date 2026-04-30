---
title: "IEvents.OnLoaded"
description: "Specifies the name of the user command that DIAdem executes after loading data."
---

# IEvents.OnLoaded

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: OnLoaded for Events <Navigator>

Specifies the name of the user command that DIAdem executes after loading data.

## Signature

```python
obj.OnLoaded
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
AddUserCommandToEvent("dd.Navigator.Events.OnLoaded","MyOnLoaded")

def MyOnLoaded():
    Txt = ""
    for Element in LoadedElementList:
        Txt = Txt + "Loaded Element: " + Element.Name + VBCrLf
    MsgBoxDisp(Txt)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="../../events/onloaded-onloaded/">Event: OnLoaded</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_OnLoaded_IEvents.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
