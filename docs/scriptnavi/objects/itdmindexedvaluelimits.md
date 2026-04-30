---
title: "ITDMIndexedValueLimits"
description: "Returns in a DataFinder the indexed value range for a property , or for an optimized custom property that is an integer or numeric data type, or for a date/time"
---

# ITDMIndexedValueLimits

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ValueLimits

Returns in a DataFinder the indexed value range for a property , or for an optimized custom property that is an integer or numeric data type, or for a date/time property.

## Python example

```python
oMyProperties = dd.Navigator.Display.CurrDataFinder.QueryForm.GetIndexedProperties(dd.eSearchChannel)
oMyValueLimits = oMyProperties.Item("Maximum").GetValueLimits
dd.MsgBoxDisp (oMyValueLimits.Min)
```

```python
MyDataFinder = dd.Navigator.Display.CurrDataFinder.GetDataFinder()
MyProperties = MyDataFinder.GetIndexedProperties(dd.eSearchFile)
MyAdaptiveQuery = MyDataFinder.CreateQuery(dd.eAdvancedQuery)
MyAdaptiveQuery.Conditions.Add (dd.eSearchFile, "fullpath", "=", dd.DataReadPath + "*")
dd.Navigator.Display.CurrDataFinder.QueryForm.SetCurrQuery(MyAdaptiveQuery)
MyCreateTimes = MyProperties.Item("createTime").GetValueLimits(MyAdaptiveQuery)
dd.MsgBoxDisp (dd.RTT(MyCreateTimes.Max.Variantdate))
dd.MsgBoxDisp (dd.RTT(MyCreateTimes.Min.Variantdate))
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmindexedvaluelimits-max/">Max</a> | <a href="../../properties/itdmindexedvaluelimits-min/">Min</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmindexedproperty/">IndexedProperty</a>.<a href="../../methods/itdmindexedproperty-getvaluelimits/">GetValueLimits</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMIndexedValueLimits.htm`*
