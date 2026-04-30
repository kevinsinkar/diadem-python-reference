---
title: "INaviDataStoreBrowser.EnableDropData"
description: "Enables you to drop data from the Data Portal into data stores to save data. Note If you drag and droop data from the Data Portal into the data browser, DIAdem "
---

# INaviDataStoreBrowser.EnableDropData

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: EnableDropData for Browser <DataStore>

Enables you to drop data from the Data Portal into data stores to save data. Note If you drag and droop data from the Data Portal into the data browser, DIAdem executes the event OnDataStoreSaving . With this event you can determine, for example, which element is selected in the Data Portal and on which file the focus in the data browser is before you save data.

## Signature

```python
obj.EnableDropData
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you drag and droop data from the Data Portal into the data browser, DIAdem executes the event <a href="../ievents-ondatastoresaving/">OnDataStoreSaving</a>. With this event you can determine, for example, which element is selected in the Data Portal and on which file the focus in the data browser is before you save data.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to the Help page <a href="#" data-unresolved="1">Working with Events in DIAdem</a> for further information.</td></tr></table>
</div>

## Python example

```python
dd.Navigator.Display.CurrDataStore.Browser.EnableDropData = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_EnableDropData_INaviDataStoreBrowser.htm`*
