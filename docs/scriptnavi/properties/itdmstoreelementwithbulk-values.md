---
title: "ITDMStoreElementWithBulk.Values"
description: "Specifies in a data store the value vector of a LocalColumn. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataSto"
---

# ITDMStoreElementWithBulk.Values

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Values for ElementWithValues <DataStore>

Specifies in a data store the value vector of a LocalColumn. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types.

## Signature

```python
obj.Values(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Only the data elements derived from the base type <span class="Monospace">AoLocalColumn</span> are <span class="Monospace">ElementWithValues &lt;DataStore&gt;</span> types.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To assign values to the <span class="Monospace">Values</span> properties, the <a href="../itdmstoreelementwithbulk-datatype/">DataType</a> property must have a valid data type.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>When working with raw data, for example if the <span class="Monospace">sequence_representation</span> property has the value <span class="Monospace">RawLinear</span>, only use the <span class="Monospace">values</span> property to read or set the raw data. The associated scaling parameters are located in the <span class="Monospace">generation_parameters</span> property.<br attr="ext"/>Implicit LocalColumns store these parameters in the <span class="Monospace">values</span> property. If the <span class="Monospace">sequence_representation</span> property has the value <span class="Monospace">ImplicitConstant</span>, the <span class="Monospace">size</span> property has a value of 1, for the value <span class="Monospace">ImplicitLinear</span> it has a value of 2, and for the value <span class="Monospace">Implicit_saw</span> it has the value of 3. The respective generating parameters are located at the appropriate positions of the <span class="Monospace">Values</span> property. The number of the values to be generated determines the <span class="Monospace">number_of_rows</span> property of the associated submatrix. The <span class="Monospace">sequence_representation</span> property can contain the following values in ASAM-ODS:<br attr="ext"/><br attr="ext"/>
<table class="Borderless">
<tr>
<td width="150"><strong>Property</strong></td>
<td><strong>Value</strong></td>
</tr>
<tr>
<td width="150"><span class="Monospace">Explicit</span></td>
<td>0</td>
</tr>
<tr>
<td width="150"><span class="Monospace">ImplicitConstant</span></td>
<td>1</td>
</tr>
<tr>
<td width="150"><span class="Monospace">ImplicitLinear</span></td>
<td>2</td>
</tr>
<tr>
<td width="150"><span class="Monospace">ImplicitSaw</span></td>
<td>3</td>
</tr>
<tr>
<td width="150"><span class="Monospace">RawLinear</span></td>
<td>4</td>
</tr>
<tr>
<td width="150"><span class="Monospace">RawPolynomial</span></td>
<td>5</td>
</tr>
<tr>
<td width="150"><span class="Monospace">Formula</span> (not used in ASAM ODS 5.2.0)</td>
<td>6</td>
</tr>
<tr>
<td width="150"><span class="Monospace">ExternalComponent</span></td>
<td>7</td>
</tr>
<tr>
<td width="150"><span class="Monospace">RawLinearExternal</span></td>
<td>8</td>
</tr>
<tr>
<td width="150"><span class="Monospace">RawPolynomialExternal</span></td>
<td>9</td>
</tr>
<tr>
<td width="150"><span class="Monospace">RawLinearCalibrated</span></td>
<td>10</td>
</tr>
<tr>
<td width="150"><span class="Monospace">RawLinearCalibratedExternal</span></td>
<td>11</td>
</tr>
</table>
</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Explicit` | 0 |  |
| `ExternalComponent` | 7 |  |

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
<p><a href="../itdmstoreelementwithbulk-size/">Size</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Values_ITDMStoreElementWithBulk.htm`*
