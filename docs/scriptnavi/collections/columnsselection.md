---
title: "ColumnsSelection"
description: "Collection of the columns selected in the search results of a DataFinder or of a data store."
---

# ColumnsSelection

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: ColumnsSelection

Collection of the columns selected in the search results of a DataFinder or of a data store.

## Python example

```python
dd.Navigator.Display.OpenDataFinder("My DataFinder")
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchFile
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Brake*")
oMyQueryForm.Search()
oMyResultsList = oMyCurrDataProvider.ResultsList
dd.WndShow("NAVIGATOR", "SHOW")
dd.InterActionOn("Select one column in the search results")
dd.WndShow("SCRIPT", "SHOW")
ColumnsSelection = oMyResultsList.ColumnsSelection
if ColumnsSelection.IsKindOf(dd.eColumnsSelection) :
    for Column in ColumnsSelection:
        dd.MsgBoxDisp(Column.Property)
else:
    dd.MsgBoxDisp("No Column Selected")
```

```python
dd.Data.Root.Clear()
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oMyCurrDataProvider = dd.Navigator.Display.CurrDataStore
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = "measurement"
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add("measurement","Name","=","TL2700_1")
oMyQueryForm.Search()
dd.WndShow("NAVIGATOR")
dd.InteractionOn("Please select one or more results list columns")
dd.WndShow("SCRIPT")
oMyResultsList = oMyCurrDataProvider.ResultsList
oMySelectedColumns = oMyResultsList.ColumnsSelection
for MySelectedColumn in oMySelectedColumns:
    dd.MsgBoxDisp("Column Property: " + MySelectedColumn.Property + "\r\n" + "Column Type: " + MySelectedColumn.Type)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmresultsdisplaycolumnsselection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmresultsdisplaycolumnsselection-iskindof/">IsKindOf</a> | <a href="../../methods/itdmresultsdisplaycolumnsselection-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/inavidatafinderresultdisplay/">ResultsList &lt;DataFinder&gt;</a>.<a href="../../properties/inavidatafinderresultdisplay-columnsselection/">ColumnsSelection</a> | <a href="../../objects/inavidatastoreresultdisplay/">ResultsList &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastoreresultdisplay-columnsselection/">ColumnsSelection</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMResultsDisplayColumnsSelection.htm`*
