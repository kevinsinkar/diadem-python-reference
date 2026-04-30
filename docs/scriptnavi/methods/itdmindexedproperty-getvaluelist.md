---
title: "ITDMIndexedProperty.GetValueList"
description: "Returns in a DataFinder the list of indexed values for a text property or for an optimized text custom property."
---

# ITDMIndexedProperty.GetValueList

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetValueList for IndexedProperty

Returns in a DataFinder the list of indexed values for a text property or for an optimized text custom property.

## Signature

```python
return_value = obj.GetValueList([AdvancedQuery], [Prefix])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the property <a href="../../properties/inavidatafinderqueryform-valuemaxcount/">ValueMaxCount for QueryForm</a> to specify the maximum number of indexed values to be displayed in DIAdem NAVIGATOR. Use the property <a href="../../properties/itdmdatafinder-valuemaxcount/">ValueMaxCount for DataFinder</a> to specify the maximum number of indexed values in a search without the interface.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <a href="#" data-unresolved="1">Set statement</a> to assign objects to a variable and to make it easier to access these objects.</td></tr></table>
</div>

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyProperties = oMyDataFinder.GetIndexedProperties(dd.eSearchChannel)
oMyValues = oMyProperties.Item("Name").GetValueList
while (oMyValues.IsIncomplete):
    oMyDataFinder.ValueMaxCount = oMyDataFinder.ValueMaxCount + 100
    oMyValues = oMyProperties("Name").GetValueList
```

```python
MyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
MyProperties = MyDataFinder.GetIndexedProperties(dd.eSearchChannel)
MyAdaptiveQuery = dd.Navigator.ConnectDataFinder("My DataFinder").CreateQuery(dd.eAdvancedQuery)
MyAdaptiveQuery.Conditions.Add(dd.eSearchFile, "fullpath", "=", dd.DataReadPath + "*")
MyChnNames = MyProperties.Item("name").GetValueList(MyAdaptiveQuery)
for i in range( 1, MyChnNames.Count+1):
    MyOutput = MyOutput + "; " + MyChnNames.Values(i)
print(MyOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetValueList_ITDMIndexedProperty.htm`*
