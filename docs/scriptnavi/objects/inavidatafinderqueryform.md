---
title: "INaviDataFinderQueryForm"
description: "The QueryForm object provides the search input area of a DataFinder. Use the Search method for the current search. The Search Results contains the results of th"
---

# INaviDataFinderQueryForm

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: QueryForm <DataFinder>

The QueryForm object provides the search input area of a DataFinder. Use the Search method for the current search. The Search Results contains the results of the search.

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
<p><a href="../../properties/inavidatafinderqueryform-conditions/">Conditions</a> | <a href="../../properties/inavidatafinderqueryform-mode/">Mode</a> | <a href="../../properties/inavidatafinderqueryform-resultsmode/">ResultsMode</a> | <a href="../../properties/inavidatafinderqueryform-returntype/">ReturnType</a> | <a href="../../properties/inavidatafinderqueryform-text/">Text</a> | <a href="../../properties/inavidatafinderqueryform-valuemaxcount/">ValueMaxCount</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/inavidatafinderqueryform-clear/">Clear</a> | <a href="../../methods/inavidatafinderqueryform-clearhistory/">ClearHistory</a> | <a href="../../methods/inavidatafinderqueryform-getcurrquery/">GetCurrQuery</a> | <a href="../../methods/inavidatafinderqueryform-getindexedproperties/">GetIndexedProperties</a> | <a href="../../methods/inavidatafinderqueryform-refreshall/">RefreshAll</a> | <a href="../../methods/inavidatafinderqueryform-search/">Search</a> | <a href="../../methods/inavidatafinderqueryform-setcurrquery/">SetCurrQuery</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idatafinderdisplay/">DataFinderDisplay</a>.<a href="../../properties/idatafinderdisplay-queryform/">QueryForm</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_INaviDataFinderQueryForm.HTM`*
