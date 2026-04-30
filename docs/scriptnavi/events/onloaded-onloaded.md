---
title: "OnLoaded.OnLoaded"
description: "Is triggered in DIAdem NAVIGATOR after you load data. The event starts the user command that you assigned to the OnLoaded for Events <Navigator> property."
---

# OnLoaded.OnLoaded

!!! abstract "Event &middot; `ScriptNavi.chm`"
    Event: OnLoaded

Is triggered in DIAdem NAVIGATOR after you load data. The event starts the user command that you assigned to the OnLoaded for Events <Navigator> property.

## Signature

```python
obj.OnLoaded
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to one event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If DIAdem does not execute the events <span class="Monospace">OnDataStoreLoading</span> or <span class="Monospace">OnFileLoading</span>, because you assigned the value <span class="Monospace">SkipLoadCmd</span> to the <span class="Monospace">NaviLoadControl</span> parameter, DIAdem cannot execute the event <span class="Monospace">OnLoaded</span>.</td></tr></table>
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
<p class="body"><a href="../onfileloading-onfileloading/">Event: OnFileLoading</a> | <a href="../ondatastoreloading-ondatastoreloading/">Event: OnDataStoreLoading</a> | <a href="../../objects/ievents/">Object: Events</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/events/navigator_event_OnLoaded.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
