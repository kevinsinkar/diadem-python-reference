---
title: "INavigator.LoadData"
description: "Loads one or more elements from the search results, the file browser, or the data browser into the Data Portal, or registers these elements in the Data Portal."
---

# INavigator.LoadData

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: LoadData for Navigator

Loads one or more elements from the search results, the file browser, or the data browser into the Data Portal, or registers these elements in the Data Portal.

## Signature

```python
return_value = obj.LoadData(ImportObject, [ImportAction], [ImportSettings])
```

## Python example

```python
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oMyDataProvider = dd.Navigator.Display.CurrDataStore.GetDataStore()
oMyElements = dd.Navigator.Display.CurrDataStore.Browser.SelectedElements

oMyPropertyImportSet = dd.Navigator.Settings.LoadPropertyImportSet("D:\\MyPropertyImportSet.tdl", oMyDataProvider)
dd.Navigator.LoadData(oMyElements,"Load", oMyPropertyImportSet)
```

```python
oMyDataProvider = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyElements = oMyDataProvider.RootElements(1).Children(1).Children
oMyPropertyImportSet = dd.Navigator.Settings.CreatePropertyImportSet(oMyDataProvider)
oMyLoadedElements = dd.Navigator.LoadData(oMyElements, "Load", oMyPropertyImportSet)
```

```python
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oMyDataProvider = dd.Navigator.Display.CurrDataStore.GetDataStore()
oMyElements = dd.Navigator.Display.CurrDataStore.Browser.SelectedElements

oMyImportParameter = dd.Navigator.Settings.CreateImportParameter()
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingOnFirstAccess
oMyImportParameter.ImportMode = dd.eLoad
oMyImportParameter.PropertyHandling.AutoUpdateChnCharacteristics = True
oMyImportParameter.PropertyHandling.InheritanceMode = dd.ePropInheritanceCopyToChannelLevel

dd.Navigator.LoadData(oMyElements, oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p class="body"><a href="#" data-unresolved="1">Objects Overview</a> | <a href="../../collections/elementlist/">Elements</a> | <a href="../../objects/isusielement/">Element</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p></div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_LoadData_INavigator.htm`*
