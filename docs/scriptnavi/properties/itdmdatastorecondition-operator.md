---
title: "ITDMDataStoreCondition.Operator"
description: "Specifies the operator that DIAdem uses in a data store for a search condition."
---

# ITDMDataStoreCondition.Operator

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Operator for Condition <DataStore>

Specifies the operator that DIAdem uses in a data store for a search condition.

## Signature

```python
obj.Operator
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you are searching for a date property, you can use the operators <span class="Monospace">=</span>, <span class="Monospace">&lt;=</span>, <span class="Monospace">&gt;=</span> and <span class="Monospace">#</span>. If you use the <span class="Monospace">#</span> operator, you can search for the following fixed time domains: <span class="Monospace">Today</span>, <span class="Monospace">Yesterday</span>, <span class="Monospace">LastSevenDays</span>, <span class="Monospace">LastFourteenDays</span>, or <span class="Monospace">LastThirtyDays</span>. If you search for text, you only can use the <span class="Monospace">=</span> operator and the <span class="Monospace">&lt;&gt;</span> operator. You can use the following operators to search for all other properties: <span class="Monospace">=</span>, <span class="Monospace">&lt;&gt;</span>, <span class="Monospace">&lt;</span>, <span class="Monospace">&gt;</span>, <span class="Monospace">&lt;=</span>, and <span class="Monospace">&gt;=</span>. Refer to the Help page <a href="#" data-unresolved="1">Notes on Searching for Data (Data Stores)</a> for information on searching in data stores.</td></tr></table>
</div>

## Python example

```python
oMyQuery = dd.Navigator.Display.CurrDataStore.QueryForm.GetCurrQuery()
dd.MsgBoxDisp("Operator: " + oMyQuery.Conditions(1).Operator)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Operator_ITDMDataStoreCondition.htm`*
