---
title: "IEvents.OnShowingContextMenu"
description: "Specifies the name of the user command that DIAdem executes when you open a context menu in DIAdem NAVIGATOR."
---

# IEvents.OnShowingContextMenu

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: OnShowingContextMenu for Events <Navigator>

Specifies the name of the user command that DIAdem executes when you open a context menu in DIAdem NAVIGATOR.

## Signature

```python
obj.OnShowingContextMenu
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
AddUserCommandToEvent("dd.Navigator.Events.OnShowingContextMenu","MyOnShowingContextMenu")

AddUserCommandToEvent("dd.Navigator.Events.OnContextMenuPointSelected","MyOnContextMenuPointSelected")

def MyOnShowingContextMenu(ParentObj, MenuPoints):
    if (ParentObj.IsKindOf(eDataBrowser)):  # eDataStoreBrowser or eDataFinderBrowser
        MenuPoints.Add("My Browser Menu Point", 1)
        if (ParentObj.IsKindOf(eDataFinderBrowser)):  # eDataStoreBrowser or eDataFinderBrowser
            MenuPoints.Add("My DataFinder Browser Menu Point", 2)
        elif (ParentObj.IsKindOf(eDataStoreBrowser)):  # eDataStoreBrowser or eDataFinderBrowser
            MenuPoints.Add("My DataStore Browser Menu Point", 3)
    elif (ParentObj.IsKindOf(eDataResultsList)):  # eDataStoreResultsList or eDataFinderResultsList
        MenuPoints.Add("My Results List Menu Point", 4)
        if (ParentObj.IsKindOf(eDataFinderResultsList)):  # eDataStoreResultsList or eDataFinderResultsList
            MenuPoints.Add("My DataFinder Results List Menu Point", 5)
        elif (ParentObj.IsKindOf(eDataStoreResultsList)):  # eDataStoreResultsList or eDataFinderResultsList
            MenuPoints.Add("My DataStore Results List Menu Point", 6)
    elif (ParentObj.IsKindOf(eChannelPreview)):
        MenuPoints.Add("My Preview Area Channel Menu Point", 7)
    elif (ParentObj.IsKindOf(ePropertyListPreview)):
        MenuPoints.Add("My Preview Area Properties Menu Point", 8)

def MyOnContextMenuPointSelected(ParentObj, MenuPoint):
    pass
    # select MenuPoint.ID
    # case 1 dd.MsgBox "DataStore or DataFinder Browser Entry"
    # case 2 dd.MsgBox "DataStore Browser Entry"
    # case 3 dd.MsgBox "DataFinder Browser Entry"
    # case 4 dd.MsgBox "DataStore or DataFinder ResultsList Entry"
    # case 5 dd.MsgBox "DataStore ResultsList Entry"
    # case 6 dd.MsgBox "DataFinder ResultsList Entry"
    # case 7 dd.MsgBox "Preview Area Channels Entry"
    # case 8 dd.MsgBox "Preview Area Properties Entry"
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="../../events/onshowingcontextmenu-onshowingcontextmenu/">Event: OnShowingContextMenu</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_OnShowingContextMenu_IEvents.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
