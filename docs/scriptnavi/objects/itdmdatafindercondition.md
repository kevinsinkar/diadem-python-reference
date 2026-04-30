---
title: "ITDMDataFinderCondition"
description: "The Condition object provides a row of the search parameters with a DataFinder for the advanced search."
---

# ITDMDataFinderCondition

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Condition <DataFinder>

The Condition object provides a row of the search parameters with a DataFinder for the advanced search.

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
if oMyQuery.IsKindOf(dd.eAdvancedQuery) :
    oCondition = oMyQuery.Conditions.Item(1)
    dd.MsgBoxDisp(oCondition.Property + oCondition.Operator + oCondition.Value)
else:
    dd.MsgBoxDisp("No Extended Search")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatafindercondition-name/">Name</a> | <a href="../../properties/itdmdatafindercondition-operator/">Operator</a> | <a href="../../properties/itdmdatafindercondition-orderby/">OrderBy</a> | <a href="../../properties/itdmdatafindercondition-property/">Property</a> | <a href="../../properties/itdmdatafindercondition-size/">Size</a> | <a href="../../properties/itdmdatafindercondition-type/">Type</a> | <a href="../../properties/itdmdatafindercondition-value/">Value</a> | <a href="../../properties/itdmdatafindercondition-values/">Values</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/conditions/">Conditions &lt;DataFinder&gt;</a>.<a href="../../methods/itdmdatafinderconditions-add/">Add</a> | <a href="../../collections/conditions/">Conditions &lt;DataFinder&gt;</a>.<a href="../../methods/itdmdatafinderconditions-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataFinderCondition.htm`*
