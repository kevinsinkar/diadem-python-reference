---
title: "OnDataStoreLoading.OnDataStoreLoading"
description: "Is triggered in DIAdem NAVIGATOR before data is loaded from a data store. The event starts the user command that you assigned to the OnDataStoreLoading for Even"
---

# OnDataStoreLoading.OnDataStoreLoading

!!! abstract "Event &middot; `ScriptNavi.chm`"
    Event: OnDataStoreLoading

Is triggered in DIAdem NAVIGATOR before data is loaded from a data store. The event starts the user command that you assigned to the OnDataStoreLoading for Events <Navigator> property.

## Signature

```python
obj.OnDataStoreLoading(NaviLoadControl, ElementListOrABS, ImportAction)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150"><em>Object</em></td>
<td><a href="../../objects/ievents/">Events &lt;Navigator&gt;</a><br attr="ext"/>Object with this property</td>
</tr>
<tr>
<td width="150"><em>Object</em>.OnDataStoreLoading</td>
<td>String with read and write access</td>
</tr>
<tr>
<td width="150"><em>NaviLoadControl</em></td>
<td>Specifies whether DIAdem executes the loading command. The <span class="Monospace">NaviLoadControl</span> parameter is a <a href="#" data-unresolved="1">String</a> type and it can contain the enumeration terms <span class="Monospace">ExecuteLoadCmd</span> (execute load command) or <span class="Monospace">SkipLoadCmd</span> (do not execute load command). If DIAdem does not execute the loading command, the program does not execute the <span class="Monospace">OnLoaded</span> event either.</td>
</tr>
<tr>
<td width="150"><i>ElementListOrABS</i></td>
<td>Specifies the object to load. If the <a href="../../methods/inavigator-loaddata/">LoadData</a> command triggers the event, you receive an <a href="../../collections/elementlist-2/">ElementList object</a> here. If the <a href="../../../comoff/commands/storageimport/">StorageImport</a> command triggers the event, you receive the ABS, which is a key displayed as an XML string, with which you access external data stores. If you load channels from an external data store in the recording mode, DIAdem usually records the key.</td>
</tr>
<tr>
<td width="150"><em>ImportAction</em></td>
<td>Variant<br attr="ext"/>Uses the <a href="../../objects/iimportparameterset/">ImportParameter</a> object to specify how DIAdem imports data into the Data Portal.<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  From DIAdem 2017, you can only use the <a href="../../objects/iimportparameterset/">ImportParameter</a> object for the <span class="Monospace">ImportAction</span> parameter. If you used the <span class="Monospace">OnFileLoading</span> event in scripts of earlier DIAdem versions, and the event executes a query on the text "Load", you must adjust the query as follows: <span class="Monospace">If (Instr(1, ImportAction, "Load", vbTextCompare)) Then ...</span><br attr="ext"/>This change is necessary because in DIAdem version 2017 the enumeration term <span class="Monospace">Load</span> was replaced by the terms <span class="Monospace">LoadImmediately</span>, <span class="Monospace">LoadByFirstRead</span>, and <span class="Monospace">LoadByFirstWrite</span>.</td>
</tr>
</table>
</td>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  From DIAdem 2017, you can only use the <a href="../../objects/iimportparameterset/">ImportParameter</a> object for the <span class="Monospace">ImportAction</span> parameter. If you used the <span class="Monospace">OnFileLoading</span> event in scripts of earlier DIAdem versions, and the event executes a query on the text "Load", you must adjust the query as follows: <span class="Monospace">If (Instr(1, ImportAction, "Load", vbTextCompare)) Then ...</span><br attr="ext"/>This change is necessary because in DIAdem version 2017 the enumeration term <span class="Monospace">Load</span> was replaced by the terms <span class="Monospace">LoadImmediately</span>, <span class="Monospace">LoadByFirstRead</span>, and <span class="Monospace">LoadByFirstWrite</span>.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../../../comoff/commands/addusercommandtoevent/">AddUserCommandToEvent</a> command to assign several user commands to one event. Use the <a href="../../../comoff/commands/removeusercommandfromevent/">RemoveUserCommandFromEvent</a> command to delete a single <a href="#" data-unresolved="1">user command</a> from a list of user commands which you assigned to an <a href="#" data-unresolved="1">event</a>. Assign an empty string to an event so that the event is no longer assigned to a user command.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.AddUserCommandToEvent("dd.Navigator.Events.OnDataStoreLoading","MyOnDataStoreLoading")

def MyOnDataStoreLoading(NaviLoadControl, ElementListOrABS, ImportAction):
    if (ElementListOrABS is not None):
        for Element in ElementListOrABS:
            MsgBoxDisp("Element name: " + Element.Name)
    else:
        MsgBoxDisp("Event Parameter StorageABS" + "\r\n" + ElementListOrABS)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="../onfileloading-onfileloading/">Event: OnFileLoading</a> | <a href="../onloaded-onloaded/">Event: OnLoaded</a> | <a href="../../objects/ievents/">Object: Events</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/events/navigator_event_OnDataStoreLoading.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
