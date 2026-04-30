---
title: "ITDMDataFinderConditions.Logic"
description: "Returns the logical operations of search conditions of a DataFinder in the search input area. You can connect search conditions with AND and OR. Use parentheses"
---

# ITDMDataFinderConditions.Logic

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Logic for Conditions <DataFinder>

Returns the logical operations of search conditions of a DataFinder in the search input area. You can connect search conditions with AND and OR. Use parentheses to specify the order of the evaluation.

## Signature

```python
obj.Logic
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you assign only the value OR to the property <span class="Monospace">Logic</span>, without listing the associated search conditions, DIAdem automatically connects all the existing search conditions with OR. If you assign only the value AND or no values to the property <span class="Monospace">Logic</span>, without listing the associated search conditions, DIAdem automatically connects all the existing search conditions with AND.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You must always create the search condition first before you connect the search conditions with a logical operator.</td></tr></table>
</div>

## Python example

```python
oMyQuery = dd.Navigator.ConnectDataFinder("My DataFinder").CreateQuery(dd.eAdvancedQuery)
oMyQuery.Conditions.Add(dd.eSearchFile,"createTime","<=",dd.CreateTime(2007,10,23,23,59,59,0,0,0))
oMyQuery.Conditions.Add(dd.eSearchFile,"Filename","=","test or example")
oMyQuery.Conditions.Add(dd.eSearchFile,"dataPluginName","=","TDM or TDMS")
oMyQuery.Conditions.Logic = ("(C1 and C2) or C3")
dd.Navigator.Display.CurrDataFinder.QueryForm.SetCurrQuery(oMyQuery)
dd.Navigator.Display.CurrDataFinder.QueryForm.Search()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Logic_ITDMDataFinderConditions.htm`*
