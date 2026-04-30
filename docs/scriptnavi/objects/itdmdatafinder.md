---
title: "ITDMDataFinder"
description: "The DataFinder object provides a DataFinder without using the DIAdem NAVIGATOR interface. You can run a Quick search and an Advanced search with the DataFinder "
---

# ITDMDataFinder

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: DataFinder

The DataFinder object provides a DataFinder without using the DIAdem NAVIGATOR interface. You can run a Quick search and an Advanced search with the DataFinder object. Use the properties ResultsElements and ResultsProperties to access the search results.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the ‎‏<a href="../idatafinderdisplay/">DataFinderDisplay</a> object to execute a search on the Navigator interface.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Clear()
oMyCurrDataProvider = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyCurrDataProvider.CreateQuery(dd.eTextQuery)
oMyQuery.Text = "Brake*"
oMyCurrDataProvider.SearchElements(oMyQuery)
oMyResults = oMyCurrDataProvider.ResultsElements
for Element in oMyResults:
    Output = Output + "\r\n" + Element.Name
dd.MsgBoxDisp("Results Elements: " + Output)
dd.Navigator.LoadData(oMyResults)
```

```python
dd.Data.Root.Clear()
oMyCurrDataProvider = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyCurrDataProvider.CreateQuery(dd.eAdvancedQuery)
oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","TR_M17_QT_*")
oMyConditions.Add(dd.eSearchChannelGroup,"Test_Status","=","fail")
oMyConditions.Add(dd.eSearchChannel,"maximum",">","45")
oMyConditions.Add(dd.eSearchChannel,"minimum","<",23)
oMyConditions.Add(dd.eSearchChannel,"Limit_High","=",50)
oMyConditions.Add(dd.eSearchChannel,"unit_string","=","+deg;C")
oMyCurrDataProvider.SearchElements(oMyQuery)
oMyResults = oMyCurrDataProvider.ResultsElements
dd.Navigator.LoadData(oMyResults)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatafinder-indexer/">Indexer</a> | <a href="../../properties/itdmdatafinder-name/">Name</a> | <a href="../../properties/itdmdatafinder-resultselements/">ResultsElements</a> | <a href="../../properties/itdmdatafinder-resultsproperties/">ResultsProperties</a> | <a href="../../properties/itdmdatafinder-valuemaxcount/">ValueMaxCount</a> | <a href="../../properties/itdmdatafinder-version/">Version</a> | <a href="../../properties/itdmdatafinder-versionnumber/">VersionNumber</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatafinder-createelementlist/">CreateElementList</a> | <a href="../../methods/itdmdatafinder-createquery/">CreateQuery</a> | <a href="../../methods/itdmdatafinder-createresultscolumns/">CreateResultsColumns</a> | <a href="../../methods/itdmdatafinder-getcoserverparameters/">GetCoServerParameters</a> | <a href="../../methods/itdmdatafinder-getindexedproperties/">GetIndexedProperties</a> | <a href="../../methods/itdmdatafinder-getsettings/">GetSettings</a> | <a href="../../methods/itdmdatafinder-loadquery/">LoadQuery</a> | <a href="../../methods/itdmdatafinder-loadresultscolumns/">LoadResultsColumns</a> | <a href="../../methods/itdmdatafinder-refresh/">Refresh</a> | <a href="../../methods/itdmdatafinder-reset/">Reset</a> | <a href="../../methods/itdmdatafinder-savequery/">SaveQuery</a> | <a href="../../methods/itdmdatafinder-searchelements/">SearchElements</a> | <a href="../../methods/itdmdatafinder-searchproperties/">SearchProperties</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idatafinderdisplay/">DataFinderDisplay</a>.<a href="../../methods/idatafinderdisplay-getdatafinder/">GetDataFinder</a> | <a href="../inavigator/">Navigator</a>.<a href="../../methods/inavigator-connectdatafinder/">ConnectDataFinder</a> | <a href="../inavigator/">Navigator</a>.<a href="../../methods/inavigator-connectdatafinderbyparameter/">ConnectDataFinderByParameter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../idatafinderdisplay/">DataFinderDisplay</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataFinder.htm`*
