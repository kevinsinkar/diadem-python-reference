---
title: "ITDMDataStore"
description: "The DataStore object provides an ASAM data store without using the DIAdem NAVIGATOR interface. Note Use the DataStoreDisplay object to execute an interface sear"
---

# ITDMDataStore

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: DataStore

The DataStore object provides an ASAM data store without using the DIAdem NAVIGATOR interface. Note Use the DataStoreDisplay object to execute an interface search in the Navigator.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../idatastoredisplay/">DataStoreDisplay</a> object to execute an interface search in the Navigator.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")

oMyQuery = oMyDataStore.CreateQuery(dd.eDataStoreQuery)
oMyQuery.ReturnType = "measurement"
oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add("MeaQuantity","minimum",">=","900")
oMyConditions.Logic = "C1"

oMyDataStore.SearchElements(oMyQuery)
oMyResults = oMyDataStore.ResultsElements
dd.Navigator.LoadData(oMyResults, "Load", None)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatastore-model/">Model</a> | <a href="../../properties/itdmdatastore-name/">Name</a> | <a href="../../properties/itdmdatastore-parameters/">Parameters</a> | <a href="../../properties/itdmdatastore-pluginname/">PluginName</a> | <a href="../../properties/itdmdatastore-resultselements/">ResultsElements</a> | <a href="../../properties/itdmdatastore-resultsproperties/">ResultsProperties</a> | <a href="../../properties/itdmdatastore-rootelements/">RootElements</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatastore-close/">Close</a> | <a href="../../methods/itdmdatastore-createelement/">CreateElement</a> | <a href="../../methods/itdmdatastore-createelementlist/">CreateElementList</a> | <a href="../../methods/itdmdatastore-createquery/">CreateQuery</a> | <a href="../../methods/itdmdatastore-createresultscolumns/">CreateResultsColumns</a> | <a href="../../methods/itdmdatastore-deleteelement/">DeleteElement</a> | <a href="../../methods/itdmdatastore-getbrowsesettings/">GetBrowseSettings</a> | <a href="../../methods/itdmdatastore-getcontext/">GetContext</a> | <a href="../../methods/itdmdatastore-getcoserverparameters/">GetCoServerParameters</a> | <a href="../../methods/itdmdatastore-getelementbydatachannel/">GetElementByDataChannel</a> | <a href="../../methods/itdmdatastore-getelementbykey/">GetElementByKey</a> | <a href="../../methods/itdmdatastore-getelementlist/">GetElementList</a> | <a href="../../methods/itdmdatastore-getelementproperties/">GetElementProperties</a> | <a href="../../methods/itdmdatastore-getpropertyvalues/">GetPropertyValues</a> | <a href="../../methods/itdmdatastore-ismodified/">IsModified</a> | <a href="../../methods/itdmdatastore-isquerysupported/">IsQuerySupported</a> | <a href="../../methods/itdmdatastore-isvalid/">IsValid</a> | <a href="../../methods/itdmdatastore-loadquery/">LoadQuery</a> | <a href="../../methods/itdmdatastore-loadresultscolumns/">LoadResultsColumns</a> | <a href="../../methods/itdmdatastore-refresh/">Refresh</a> | <a href="../../methods/itdmdatastore-save/">Save</a> | <a href="../../methods/itdmdatastore-savequery/">SaveQuery</a> | <a href="../../methods/itdmdatastore-searchelements/">SearchElements</a> | <a href="../../methods/itdmdatastore-searchproperties/">SearchProperties</a> | <a href="../../methods/itdmdatastore-setbrowsesettings/">SetBrowseSettings</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idatafileheaderaccess/">DataFileHeaderAccess</a>.<a href="../../methods/idatafileheaderaccess-open/">Open</a> | <a href="../idatastoredisplay/">DataStoreDisplay</a>.<a href="../../methods/idatastoredisplay-getdatastore/">GetDataStore</a> | <a href="../inavigator/">Navigator</a>.<a href="../../methods/inavigator-connectdatastore/">ConnectDataStore</a> | <a href="../inavigator/">Navigator</a>.<a href="../../methods/inavigator-connectdatastorebyparameter/">ConnectDataStoreByParameter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataStore.htm`*
