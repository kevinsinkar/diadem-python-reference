---
title: "ITDMStoreElementWithBulk"
description: "The ElementWithValues object provides a data element in a data store for accessing bulk data. Note Only the data elements derived from the base type AoLocalColu"
---

# ITDMStoreElementWithBulk

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ElementWithValues <DataStore>

The ElementWithValues object provides a data element in a data store for accessing bulk data. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Only the data elements derived from the base type <span class="Monospace">AoLocalColumn</span> are <span class="Monospace">ElementWithValues &lt;DataStore&gt;</span> types.</td></tr></table>
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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmstoreelementwithbulk-children/">Children</a> | <a href="../../properties/itdmstoreelementwithbulk-datatype/">DataType</a> | <a href="../../properties/itdmstoreelementwithbulk-displayname/">DisplayName</a> | <a href="../../properties/itdmstoreelementwithbulk-flags/">Flags</a> | <a href="../../properties/itdmstoreelementwithbulk-instancekey/">InstanceKey</a> | <a href="../../properties/itdmstoreelementwithbulk-name/">Name</a> | <a href="../../properties/itdmstoreelementwithbulk-parent/">Parent</a> | <a href="../../properties/itdmstoreelementwithbulk-properties/">Properties</a> | <a href="../../properties/itdmstoreelementwithbulk-references/">References</a> | <a href="../../properties/itdmstoreelementwithbulk-size/">Size</a> | <a href="../../properties/itdmstoreelementwithbulk-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmstoreelementwithbulk-getdatafinderinfo/">GetDataFinderInfo</a> | <a href="../../methods/itdmstoreelementwithbulk-iskindof/">IsKindOf</a> | <a href="../../methods/itdmstoreelementwithbulk-isvalid/">IsValid</a> | <a href="../../methods/itdmstoreelementwithbulk-refresh/">Refresh</a> | <a href="../../methods/itdmstoreelementwithbulk-save/">Save</a> | <a href="../../methods/itdmstoreelementwithbulk-setvalues/">SetValues</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavidatastorebrowser/">Browser &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastorebrowser-focusedelement/">FocusedElement</a> | <a href="../itdmbrowsesettings/">BrowseSettings</a>.<a href="../../methods/itdmbrowsesettings-getparent/">GetParent</a> | <a href="../idatastorecell/">Cell &lt;DataStore&gt;</a>.<a href="../../properties/idatastorecell-element/">Element</a> | <a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-createelement/">CreateElement</a> | <a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-getelementbydatachannel/">GetElementByDataChannel</a> | <a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-getelementbykey/">GetElementByKey</a> | <a href="../itdmstoreelement/">Element &lt;DataStore&gt;</a>.<a href="../../properties/itdmstoreelement-parent/">Parent</a> | <a href="../../collections/elementlist-2/">ElementList &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelementlist-item/">Item</a> | <a href="../../collections/elements/">Elements &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelements-add/">Add</a> | <a href="../../collections/elements/">Elements &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelements-addreference/">AddReference</a> | <a href="../../collections/elements/">Elements &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelements-item/">Item</a> | <a href="../../collections/elementsselection-2/">ElementsSelection &lt;DataStore&gt;</a>.<a href="../../methods/idatastoreresultsdisplayelementsselection-item/">Item</a> | <a href="./">ElementWithValues &lt;DataStore&gt;</a>.<a href="../../properties/itdmstoreelementwithbulk-parent/">Parent</a> | <a href="../../collections/freeelementlist-2/">FreeElementList &lt;DataStore&gt;</a>.<a href="../../methods/itdmfreestoreelementlist-add/">Add</a> | <a href="../../collections/freeelementlist-2/">FreeElementList &lt;DataStore&gt;</a>.<a href="../../methods/itdmfreestoreelementlist-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMStoreElementWithBulk.htm`*
