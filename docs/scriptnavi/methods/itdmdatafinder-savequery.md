---
title: "ITDMDataFinder.SaveQuery"
description: "Saves in a DataFinder the current query in a file with the filename extension .tdq ."
---

# ITDMDataFinder.SaveQuery

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: SaveQuery for DataFinder

Saves in a DataFinder the current query in a file with the filename extension .tdq .

## Signature

```python
obj.SaveQuery(FileName, Query, ResultsColumns)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <a href="../idatafinderdisplay-savequeryinfoset/">SaveQueryInfoSet</a> method instead of the <span class="Monospace">SaveQuery</span> method if you want to work on the DIAdem NAVIGATOR interface. Use the <span class="Monospace">SaveQueryInfoSet</span> method to also save the configuration of the search results list.</td></tr></table>
</div>

## Python example

```python
#Creating a tdq file with result columns
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchFile

oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchChannel,"maximum","<",10)
oMyConditions.Add(dd.eSearchChannel,"minimum",">",6)
oMyConditions.Logic = "C1 and C2"

oMyResultsColumns = oMyDataFinder.CreateResultsColumns()
oMyResultsColumns.RemoveAll()
oMyResultsColumns.Add(dd.eSearchChannel, "maximum")
oMyResultsColumns.Add(dd.eSearchChannel, "minimum")

oMyDataFinder.SaveQuery("D:\\MyNewQuery.tdq", oMyQuery, oMyResultsColumns)
```

```python
#Using the saved tdq file/result columns
oMyResultsColumns = oMyDataFinder.LoadResultsColumns("D:\\MyNewQuery.tdq")
oMyQuery = oMyDataFinder.LoadQuery("D:\\MyNewQuery.tdq")
oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumns, 100)
oMyResults = oMyDataFinder.ResultsProperties
dd.Navigator.LoadProperty(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_SaveQuery_ITDMDataFinder.htm`*
