---
title: "IDataFinderDisplay"
description: "The Display provides an open DataFinder. You can run a Quick search and an Advanced search with a DataFinder. You run the search on the DIAdem NAVIGATOR interfa"
---

# IDataFinderDisplay

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: DataFinderDisplay

The Display provides an open DataFinder. You can run a Quick search and an Advanced search with a DataFinder. You run the search on the DIAdem NAVIGATOR interface. To execute a search, enter the search conditions ( Conditions ) into the search input area ( QueryForm ). Use the ResultsList property to access the results of a search.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../itdmdatafinder/">DataFinder</a> object to execute a search without the Navigator interface.</td></tr></table>
</div>

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchChannel
oMyConditions = oMyQueryForm.Conditions
#Setting query conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","TR_M17_QT_*")
oMyConditions.Add(dd.eSearchChannelGroup,"Test_Status","=","fail")
oMyConditions.Add(dd.eSearchChannel,"maximum",">","45")
oMyConditions.Add(dd.eSearchChannel,"minimum","<",23)
oMyConditions.Add(dd.eSearchChannel,"Limit_High","=",50)
oMyConditions.Add(dd.eSearchChannel,"unit_string","=","+deg;C")
#Searching
oMyQueryForm.Search()
oMyResults = oMyCurrDataProvider.ResultsList.ResultsElements
#Loading results into Data Portal
dd.Navigator.LoadData(oMyResults)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatafinderdisplay-browser/">Browser</a> | <a href="../../properties/idatafinderdisplay-datafinderversion/">DataFinderVersion</a> | <a href="../../properties/idatafinderdisplay-datafinderversionnumber/">DataFinderVersionNumber</a> | <a href="../../properties/idatafinderdisplay-name/">Name</a> | <a href="../../properties/idatafinderdisplay-queryform/">QueryForm</a> | <a href="../../properties/idatafinderdisplay-resultslist/">ResultsList</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatafinderdisplay-getcoserverparameters/">GetCoServerParameters</a> | <a href="../../methods/idatafinderdisplay-getdatafinder/">GetDataFinder</a> | <a href="../../methods/idatafinderdisplay-iskindof/">IsKindOf</a> | <a href="../../methods/idatafinderdisplay-loadqueryinfoset/">LoadQueryInfoSet</a> | <a href="../../methods/idatafinderdisplay-savequeryinfoset/">SaveQueryInfoSet</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idisplay/">Display</a>.<a href="../../properties/idisplay-currdatafinder/">CurrDataFinder</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a> | <a href="../itdmdatafinder/">DataFinder</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataFinderDisplay.htm`*
