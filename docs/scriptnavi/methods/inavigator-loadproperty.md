---
title: "INavigator.LoadProperty"
description: "Loads the property values from the results of a search in a DataFinder or a data store as channels into the Data Portal."
---

# INavigator.LoadProperty

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: LoadProperty for Navigator

Loads the property values from the results of a search in a DataFinder or a data store as channels into the Data Portal.

## Signature

```python
return_value = obj.LoadProperty(PathOrIndex, Elements, [ImportAction])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you use the <span class="Monospace">ImportParameter</span> object for the <span class="Monospace">ImportAction</span> parameter, the <span class="Monospace">LoadProperty</span> command supports the properties <a href="../../properties/iimportparameterset-importmode/">ImportMode</a>, <a href="../../properties/iimportparameterset-loadreturnmode/">LoadReturnMode</a>, and <a href="../../properties/iimportparameterset-appendcheckgroupname/">AppendCheckGroupName</a>. The method ignores all other properties of the object.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  When DIAdem generates a channel in the Data Portal, the program assigns values to the following channel properties:<ul><li><span class="Monospace">Data storage origin</span>: Specifies the name of the DataFinder or data store from which DIAdem loads the data.</li><li><span class="Monospace">Data source type</span>: Specifies the type of the transferred element.</li><li><span class="Monospace">Source context</span>: Specifies which property to load.</li></ul></td></tr></table>
</div>

## Python example

```python
oMyAdvancedQuery = dd.Navigator.ConnectDataFinder("My DataFinder").CreateQuery(dd.eAdvancedQuery)
oMyAdvancedQuery.Conditions.Add(dd.eSearchChannel,"maximum",">",5)
oMyAdvancedQuery.ReturnType = dd.eSearchChannel
dd.Navigator.Display.CurrDataFinder.QueryForm.SetCurrQuery(oMyAdvancedQuery)
dd.Navigator.Display.CurrDataFinder.QueryForm.Search()
dd.Navigator.LoadProperty ("maximum",dd.Navigator.Display.CurrDataFinder.ResultsList.ResultsElements)
```

```python
oMyResultsList = dd.Navigator.Display.CurrDataStore.ResultsList
oReturnType = dd.Navigator.Display.CurrDataStore.QueryForm.GetCurrQuery().ReturnType
for oMySelection in oMyResultsList.Selection:
    dd.Navigator.LoadProperty(oMySelection.GetPath(oReturnType),oMyResultsList.ResultsElements)
```

```python
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add(dd.eSearchChannel,"maximum",">=","10")
oMyConditions.Logic = "C1"

oMyResultsColumns = oMyDataFinder.CreateResultsColumns()
oMyResultsColumns.RemoveAll()
oMyResultsColumns.Add(dd.eSearchChannelGroup, "name")
oMyResultsColumns.Add(dd.eSearchFile, "fileName")
oMyResultsColumns.Add(dd.eSearchFile, "folder")
oMyResultsColumns.Add(dd.eSearchChannel, "maximum")

oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumns)
oMyResultsProps = oMyDataFinder.ResultsProperties
dd.MsgBoxDisp("Result properties return type: " + oMyResultsProps.ReturnType)

dd.Navigator.LoadProperty(oMyResultsProps)
```

```python
oMyAdvancedQuery = dd.Navigator.ConnectDataFinder("My DataFinder").CreateQuery(dd.eAdvancedQuery)
oMyAdvancedQuery.Conditions.Add(dd.eSearchChannel,"maximum",">",5)
oMyAdvancedQuery.ReturnType = dd.eSearchChannel
dd.Navigator.Display.CurrDataFinder.QueryForm.SetCurrQuery(oMyAdvancedQuery)
dd.Navigator.Display.CurrDataFinder.QueryForm.Search()

oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
oMyImportParameter.ImportMode = dd.eAppend

dd.Navigator.LoadProperty ("maximum",dd.Navigator.Display.CurrDataFinder.ResultsList.ResultsElements, oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p></div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_LoadProperty_INavigator.htm`*
