---
title: "IEvents.OnDataProviderClosing"
description: "Specifies the name of the user command that DIAdem executes after closing a DataFinder or a data store."
---

# IEvents.OnDataProviderClosing

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: OnDataProviderClosing for Events <Navigator>

Specifies the name of the user command that DIAdem executes after closing a DataFinder or a data store.

## Signature

```python
obj.OnDataProviderClosing
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
dd.AddUserCommandToEvent("dd.Navigator.Events.OnDataProviderOpened","MyOnDataProviderOpened")
dd.AddUserCommandToEvent("dd.Navigator.Events.OnDataProviderClosing","MyOnDataProviderClosing")

def MyOnDataProviderOpened(CurrDataProvider):
    MsgBoxDisp("Opened dd.Data Provider: " + CurrDataProvider.Name)

def MyOnDataProviderClosing(CurrDataProvider):
    MsgBoxDisp("Closing dd.Data Provider: " + CurrDataProvider.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_OnDataProviderClosing_IEvents.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
