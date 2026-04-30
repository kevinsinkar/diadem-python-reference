---
title: "INavigator"
description: "The Navigator object enables access to the interface and the functions of DIAdem NAVIGATOR. Use the Navigator object to open data stores and DataFinders. You ca"
---

# INavigator

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Navigator

The Navigator object enables access to the interface and the functions of DIAdem NAVIGATOR. Use the Navigator object to open data stores and DataFinders. You can search for properties of files, channel groups, and channels in DataFinders and search for properties of tests, subtests, measurements, and measurement quantities in data stores. You can display the search results and load the results directly into the Data Portal.

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
dd.Data.Root.Clear()
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
oMyConditions.Add(dd.eSearchChannel,"unit_string","=","°C")
oMyQueryForm.Search()
oMyResults = oMyCurrDataProvider.ResultsList.ResultsElements
dd.Navigator.LoadData(oMyResults)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/inavigator-display/">Display</a> | <a href="../../properties/inavigator-events/">Events</a> | <a href="../../properties/inavigator-settings/">Settings</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/inavigator-connectdatafinder/">ConnectDataFinder</a> | <a href="../../methods/inavigator-connectdatafinderbyparameter/">ConnectDataFinderByParameter</a> | <a href="../../methods/inavigator-connectdatastore/">ConnectDataStore</a> | <a href="../../methods/inavigator-connectdatastorebyparameter/">ConnectDataStoreByParameter</a> | <a href="../../methods/inavigator-displayisactive/">DisplayIsActive</a> | <a href="../../methods/inavigator-loadchannelsbyname/">LoadChannelsByName</a> | <a href="../../methods/inavigator-loaddata/">LoadData</a> | <a href="../../methods/inavigator-loadproperty/">LoadProperty</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_INavigator.htm`*
