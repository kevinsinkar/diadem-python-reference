---
title: "ITDMDataFinderConditions.Add"
description: "Adds a new search condition to a DataFinder in an advanced search."
---

# ITDMDataFinderConditions.Add

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Add for Conditions <DataFinder>

Adds a new search condition to a DataFinder in an advanced search.

## Signature

```python
return_value = obj.Add(Type, Property, Operator, Value)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Searching for Data with the DataFinder</a> for further information about using the DataFinder to mine for data.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  DIAdem always adds new search conditions to the in the end of the logical operations line. Refer to <a href="#" data-unresolved="1">Notes on Searching with OR (DataFinder)</a> for further information on the behavior of the logical operations line.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Properties - Overview</a> for a list of the interface terms, script names, and meanings of the properties of files, groups, and channels. You need the neutral script name of a property when you use a script to search for the value of a property. You also can enter a query in the search input area in DIAdem NAVIGATOR and press &lt;Ctrl-Shift-C&gt; to find the script name of a property. Then DIAdem saves a script to the clipboard that also contains the script name of the property.</td></tr></table>
</div>

## Python example

```python
oMyQueryForm = dd.Navigator.Display.CurrDataFinder.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Conditions.Add(dd.eSearchChannel,"name","=","Speed")
oMyQueryForm.Conditions.Add(dd.eSearchChannel,"description","=","My data")
oMyQueryForm.Search()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Add_ITDMDataFinderConditions.htm`*
