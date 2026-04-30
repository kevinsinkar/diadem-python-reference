---
title: "ISUSIProperty.Default"
description: "Specifies in a DataFinder whether a property is a default property or a custom property. The Default property returns the value TRUE if the property is a defaul"
---

# ISUSIProperty.Default

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Default for Property <DataFinder>

Specifies in a DataFinder whether a property is a default property or a custom property. The Default property returns the value TRUE if the property is a default property.

## Signature

```python
obj.Default
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../../collections/indexedproperties/">IndexedProperties</a> collection to determine whether a custom property is optimized.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The <a href="../../collections/properties/">Properties</a> collection contains the base properties and the custom properties. You cannot delete base properties.</td></tr></table>
</div>

## Python example

```python
oMyResultsListProp = dd.Navigator.Display.CurrDataFinder.ResultsList.Elements(1).Properties(1)
dd.MsgBoxDisp(oMyResultsListProp.Default)
```

```python
if dd.Navigator.Display.CurrDataFinder.ResultsList.Elements(1).IsKindOf(dd.eSearchChannel) :
    oMyIndexedProperties = dd.Navigator.Display.CurrDataFinder.QueryForm.GetIndexedProperties(dd.eSearchChannel)
elif dd.Navigator.Display.CurrDataFinder.ResultsList.Elements(1).IsKindOf(dd.eSearchChannelGroup) :
    oMyIndexedProperties = dd.Navigator.Display.CurrDataFinder.QueryForm.GetIndexedProperties(dd.eSearchChannelGroup)
else:
    oMyIndexedProperties = dd.Navigator.Display.CurrDataFinder.QueryForm.GetIndexedProperties(dd.eSearchFile)
for oMyProperty in dd.Navigator.Display.CurrDataFinder.ResultsList.Elements(1).Properties:
    if oMyProperty.Default == False :
        if oMyIndexedProperties.Item(oMyProperty.Name).DataType == dd.DataTypeOptiUnknown :
            dd.MsgboxDisp (oMyProperty.Name + " is not an optimized property")
        else:
            dd.MsgboxDisp (oMyProperty.Name + " is an optimized property")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Default_ISUSIProperty.htm`*
