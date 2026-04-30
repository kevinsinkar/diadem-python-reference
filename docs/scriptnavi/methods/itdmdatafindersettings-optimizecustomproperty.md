---
title: "ITDMDataFinderSettings.OptimizeCustomProperty"
description: "Optimizes a custom property in the DataFinder configuration or deletes a custom property from the list of optimized custom properties. You can use this method o"
---

# ITDMDataFinderSettings.OptimizeCustomProperty

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: OptimizeCustomProperty for DataFinderSettings

Optimizes a custom property in the DataFinder configuration or deletes a custom property from the list of optimized custom properties. You can use this method only on the computer on which the DataFinder is active.

## Signature

```python
obj.OptimizeCustomProperty(Type, PropertyName, [OptimizedDataType])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <span class="Monospace">OptimizeCustomProperties</span> method only for the configuration of the <span class="Monospace">My DataFinder</span> DataFinder. To configure a data indexing instance in SystemLink TDM, use the SystemLink TDM HTTP API. For a description of the SystemLink TDM HTTP API, see the SystemLink Help.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you assign the value <span class="Monospace">*</span> to the <span class="Monospace">PropertyName</span> parameter and the value <span class="Monospace">DataTypeAutoIndexed</span> to the <span class="Monospace">OptimizedDataType</span> parameter, the DataFinder optimizes all indexed custom properties. If you assign the value <span class="Monospace">*</span> to the <span class="Monospace">PropertyName</span> parameter and the value <span class="Monospace">DataTypeUnknown</span> to the <span class="Monospace">OptimizedDataType</span> parameter, the DataFinder undoes the optimization of all the custom properties.</td></tr></table>
<table class="Borderless" id="table3"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you want to optimize custom properties that do not yet exist, in a script, you must specify the type of the custom properties.</td></tr></table>
<table class="Borderless" id="table5"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../../properties/itdmindexedproperty-datatype/">DataType for IndexedProperty</a> property to determine the data type of the indexed custom property.</td></tr></table>
</div>

## Python example

```python
oMyDataFinderSettings = dd.Navigator.ConnectDataFinder("My DataFinder").GetSettings()
oMyDataFinderSettings.OptimizeCustomProperty(dd.eSearchChannel, "Author_age")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_OptimizeCustomProperty_ITDMDataFinderSettings.htm`*
