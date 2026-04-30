---
title: "ITDMIndexedValueList.IsIncomplete"
description: "Specifies in a DataFinder whether the list of indexed values returned by the ValueList object is complete."
---

# ITDMIndexedValueList.IsIncomplete

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IsIncomplete for ValueList

Specifies in a DataFinder whether the list of indexed values returned by the ValueList object is complete.

## Signature

```python
obj.IsIncomplete
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>You can use the <a href="../itdmdatafinder-valuemaxcount/">ValueMaxCount</a> property to change the length of the list with the indexed values. The change becomes valid when you have refreshed the list with the <a href="../../methods/itdmindexedproperty-getvaluelist/">GetValueList</a> method.</td></tr></table>
</div>

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyProperties = oMyDataFinder.GetIndexedProperties(dd.eSearchChannel)
oMyValues = oMyProperties.Item("Name").GetValueList
while (oMyValues.IsIncomplete):
    oMyDataFinder.ValueMaxCount = oMyDataFinder.ValueMaxCount + 100
    oMyValues = oMyProperties.Item("Name").GetValueList
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IsIncomplete_ITDMIndexedValueList.htm`*
