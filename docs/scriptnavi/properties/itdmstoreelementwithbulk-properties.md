---
title: "ITDMStoreElementWithBulk.Properties"
description: "Returns the properties of a data element in a data store. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore>"
---

# ITDMStoreElementWithBulk.Properties

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Properties for ElementWithValues <DataStore>

Returns the properties of a data element in a data store. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types.

## Signature

```python
return_value = obj.Properties
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Only the data elements derived from the base type <span class="Monospace">AoLocalColumn</span> are <span class="Monospace">ElementWithValues &lt;DataStore&gt;</span> types.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>In the object oriented DIAdem NAVIGATOR interface you access bulk data of a data store with the properties <a href="../itdmstoreelementwithbulk-values/">Values</a> and <a href="../itdmstoreelementwithbulk-size/">Size</a> of the <span class="Monospace">ElementWithValues</span> object.</td></tr></table>
</div>

## Python example

```python
# Channel object of channel to be copied into ASAM data store
 # ASAM Data store object ("ASAM Browse Settings Example")
 # Element object of a measurement (Base type: aoMeasurement)
# The new channel (oMyTargetChannel) will be appended to this measurement
 # Element object of the new external channel (Base type: aoMeasurementQuantity)
 # Channel element object (Base type: aoMeasurementQuantity)
 # "Local column" element object (Base type: aoLocalColumn)
 # "Submatrix" element object (Base type: aoSubmatirx)
#------ Providing original data --------
oMyDIAdemChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyDataStore     = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyMeasurement   = oMyDataStore.RootElements(1).Children(1).Children(1)
#------ Generating new Elements --------
oSubmat          = oMyMeasurement.References("submatrices").Elements.Add("submatrix_2")
#------ Determining number of submatrix values --------
oSubmat.Properties("number_of_rows").Value = oMyDIAdemChannel.Size
oMyTargetLocalColumn = oSubmat.References("Local_Columns").Elements.Add(oMyDIAdemChannel.Name)
oMyMeaQuant = oMyMeasurement.Children.Add(oMyDIAdemChannel.Name)
oMyMeaQuant.Properties("datatype").value = "DT_DOUBLE"
oMyMeaQuant.References("local_columns").Elements.AddReference(oMyTargetLocalColumn)
#------ Writing DIAdem channel values into local column of external channel --------
oMyTargetLocalColumn.SetValues(oMyDIAdemChannel,False)
#------ Displaying first value of external channel ---------
dd.MsgBoxDisp(oMyTargetLocalColumn.Values(1))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Properties_ITDMStoreElementWithBulk.htm`*
