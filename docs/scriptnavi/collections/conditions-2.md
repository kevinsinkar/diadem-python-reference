---
title: "Conditions"
description: "Search parameters collection in a search in a data store."
---

# Conditions

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: Conditions <DataStore>

Search parameters collection in a search in a data store.

## Python example

```python
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oMyStore = dd.Navigator.Display.CurrDataStore
oMyQueryForm = oMyStore.QueryForm
oMyQueryForm.Conditions.RemoveAll()
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add("Test","Name","=","ETC")
oMyConditions.Add("Measurement","Name","=","DL")
oMyConditions.Logic = "C1 and C2"
oMyQuery = oMyQueryForm.GetCurrQuery()
if (oMyQuery.IsKindOf(dd.eDataStoreQuery)) :
    for Condition in oMyQuery.Conditions:
        dd.MsgBoxDisp("Property: " + Condition.Property + "\r\n" + "Value: " + Condition.Value)
oMyQueryForm.Search()
dd.Navigator.LoadData(oMyStore.ResultsList.ResultsElements,"Load")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatastoreconditions-count/">Count</a> | <a href="../../properties/itdmdatastoreconditions-logic/">Logic</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatastoreconditions-add/">Add</a> | <a href="../../methods/itdmdatastoreconditions-item/">Item</a> | <a href="../../methods/itdmdatastoreconditions-remove/">Remove</a> | <a href="../../methods/itdmdatastoreconditions-removeall/">RemoveAll</a> | <a href="../../methods/itdmdatastoreconditions-renumber/">Renumber</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmdatastoreadvancedquery/">AdvancedQuery &lt;DataStore&gt;</a>.<a href="../../properties/itdmdatastoreadvancedquery-conditions/">Conditions</a> | <a href="../../objects/inavidatastorequeryform/">QueryForm &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastorequeryform-conditions/">Conditions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataStoreConditions.htm`*
