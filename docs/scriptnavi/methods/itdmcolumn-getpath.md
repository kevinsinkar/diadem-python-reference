---
title: "ITDMColumn.GetPath"
description: "Returns the path which you use to access the property of the current Elements of the search results list,in the search results list of a DataFinder or a data st"
---

# ITDMColumn.GetPath

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetPath for Column

Returns the path which you use to access the property of the current Elements of the search results list,in the search results list of a DataFinder or a data store. Use the GetPath method to connect the current element to the property displayed in the Column , in the search results.

## Signature

```python
sGetPath = Object.GetPath(ReturnType)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You also can use the <span class="Monospace">GetPath</span> method to access properties of higher-ranking elements.</td></tr></table>
</div>

## Python example

```python
oMyResultsDisplay = dd.Navigator.Display.CurrDataFinder.ResultsList
oMyQueryForm = dd.Navigator.Display.CurrDataFinder.QueryForm
oMyPath = oMyResultsDisplay.Columns(1).GetPath(oMyQueryForm.GetCurrQuery().ReturnType)
dd.MsgBoxDisp (oMyResultsDisplay.Elements(1).Properties(oMyPath).Value)
```

```python
oMyResultsList = dd.Navigator.Display.CurrDataFinder.ResultsList
oReturnType = dd.Navigator.Display.CurrDataFinder.QueryForm.GetCurrQuery().ReturnType
for i in range( 1, oMyResultsList.Columns.Count+1):
    dd.Navigator.LoadProperty(oMyResultsList.Columns(i).GetPath(oReturnType),oMyResultsList.Elements)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetPath_ITDMColumn.htm`*
