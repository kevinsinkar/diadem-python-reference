---
title: "INaviDataFinderResultDisplay"
description: "The ResultsList object provides the results of an interface search in a DataFinder."
---

# INaviDataFinderResultDisplay

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ResultsList <DataFinder>

The ResultsList object provides the results of an interface search in a DataFinder.

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchChannel
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","TR_M17_QT_*")
oMyConditions.Add(dd.eSearchChannelGroup,"Test_Status","=","fail")
oMyConditions.Add(dd.eSearchChannel,"maximum",">","45")
oMyConditions.Add(dd.eSearchChannel,"minimum","<",23)
oMyConditions.Add(dd.eSearchChannel,"Limit_High","=",50)
oMyConditions.Add(dd.eSearchChannel,"unit_string","=","+deg;C")
oMyQueryForm.Search()
oMyResults = oMyCurrDataProvider.ResultsList.ResultsElements
dd.Navigator.LoadData(oMyResults)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/inavidatafinderresultdisplay-cellsselection/">CellsSelection</a> | <a href="../../properties/inavidatafinderresultdisplay-columns/">Columns</a> | <a href="../../properties/inavidatafinderresultdisplay-columnsselection/">ColumnsSelection</a> | <a href="../../properties/inavidatafinderresultdisplay-elementsselection/">ElementsSelection</a> | <a href="../../properties/inavidatafinderresultdisplay-focusedcell/">FocusedCell</a> | <a href="../../properties/inavidatafinderresultdisplay-isactive/">IsActive</a> | <a href="../../properties/inavidatafinderresultdisplay-resultselements/">ResultsElements</a> | <a href="../../properties/inavidatafinderresultdisplay-resultsproperties/">ResultsProperties</a> | <a href="../../properties/inavidatafinderresultdisplay-selection/">Selection</a> | <a href="../../properties/inavidatafinderresultdisplay-settings/">Settings</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/inavidatafinderresultdisplay-activate/">Activate</a> | <a href="../../methods/inavidatafinderresultdisplay-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idatafinderdisplay/">DataFinderDisplay</a>.<a href="../../properties/idatafinderdisplay-resultslist/">ResultsList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_INaviDataFinderResultDisplay.HTM`*
