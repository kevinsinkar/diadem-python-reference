---
title: "Properties"
description: "Collection of all properties of a data element in a data store. Use the Properties collection to access, add, or delete properties in read and write mode."
---

# Properties

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: Properties <DataStore>

Collection of all properties of a data element in a data store. Use the Properties collection to access, add, or delete properties in read and write mode.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The <span class="Monospace">Properties</span> collection contains the application properties of a data element. To access instance properties of a data element assign the value TRUE to the <a href="../../properties/itdmstoreproperties-listinstanceproperties/">ListInstanceProperties</a> property from this collection. Instance properties are user-defined properties.</td></tr></table>
</div>

## Python example

```python
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oDataMyStore = dd.Navigator.Display.CurrDataStore.GetDataStore()
oMyProperties = oDataMyStore.RootElements(1).Properties
for MyProperty in oMyProperties:
    dd.MsgBoxDisp("Property name: " + MyProperty.Name + "\r\n" + "Property value: " + MyProperty.Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmstoreproperties-count/">Count</a> | <a href="../../properties/itdmstoreproperties-listinstanceproperties/">ListInstanceProperties</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmstoreproperties-add/">Add</a> | <a href="../../methods/itdmstoreproperties-exists/">Exists</a> | <a href="../../methods/itdmstoreproperties-item/">Item</a> | <a href="../../methods/itdmstoreproperties-remove/">Remove</a> | <a href="../../methods/itdmstoreproperties-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmstoreelement/">Element &lt;DataStore&gt;</a>.<a href="../../properties/itdmstoreelement-properties/">Properties</a> | <a href="../../objects/itdmstoreelementwithbulk/">ElementWithValues &lt;DataStore&gt;</a>.<a href="../../properties/itdmstoreelementwithbulk-properties/">Properties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMStoreProperties.htm`*
