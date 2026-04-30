---
title: "ITDMDataFinderCondition.Value"
description: "Specifies the value which DIAdem searches for in an advanced search in a DataFinder."
---

# ITDMDataFinderCondition.Value

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Value for Condition <DataFinder>

Specifies the value which DIAdem searches for in an advanced search in a DataFinder.

## Signature

```python
obj.Value
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you assign an OR operator to the value of a search condition, for example, <span class="Monospace">value1 OR value2</span>, the <span class="Monospace">value</span> property contains only the first value.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Searching for Data with the DataFinder</a> for further information about using the DataFinder to mine for data.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>When you search for text properties, you can use the wildcard <span class="Monospace">?</span> for one letter and the wildcard <span class="Monospace">*</span> for any number of letters.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to the help page <a href="#" data-unresolved="1">Properties in DIAdem - Overview</a> for a table of the names, the interface terms, and the meanings of the properties of data sets, groups, and channels. The table also indicates whether you can use a property for a search in DIAdem NAVIGATOR. To find the names of properties for a search, you can also enter the search term in the search input field in DIAdem NAVIGATOR and press &lt;Ctrl-Shift-C&gt;. Then DIAdem saves a script to the clipboard that also contains the names of the properties.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you display a date/time property in the script above, you must use <span class="Monospace">Condition.Value.Variantdate</span> instead of <span class="Monospace">Condition.Value</span>.</td></tr></table>
</div>

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
if oMyQuery.IsKindOf(dd.eAdvancedQuery) :
    Conditions = oMyQuery.Conditions
    for Condition in Conditions:
        dd.MsgBoxDisp (Condition.Property + Condition.Operator + Condition.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2></h2><table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you display a date/time property in the script above, you must use <span class="Monospace">Condition.Value.Variantdate</span> instead of <span class="Monospace">Condition.Value</span>.</td></tr></table>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Value_ITDMDataFinderCondition.htm`*
