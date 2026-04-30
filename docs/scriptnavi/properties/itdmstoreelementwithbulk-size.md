---
title: "ITDMStoreElementWithBulk.Size"
description: "Specifies in a data store the number of values in the value vector of a LocalColumn. DIAdem automatically adjusts the number of values to the number of values o"
---

# ITDMStoreElementWithBulk.Size

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Size for ElementWithValues <DataStore>

Specifies in a data store the number of values in the value vector of a LocalColumn. DIAdem automatically adjusts the number of values to the number of values of the associated submatrix. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types.

## Signature

```python
obj.Size
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Only the data elements derived from the base type <span class="Monospace">AoLocalColumn</span> are <span class="Monospace">ElementWithValues &lt;DataStore&gt;</span> types.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>In implicit LocalColumns, you also can store the generation parameters in the values of the LocalColumn. The property <span class="Monospace">Size</span> then indicates how many generation parameters there are. Alternatively, the generation parameters can be stored in the <span class="Monospace">Generation_Parameters</span> property. In this case <span class="Monospace">Size</span> always returns the value 0.<br attr="ext"/>If the LocalColumns contain raw data, <span class="Monospace">Size</span> always returns the amount of the raw data in the Values vector. Parameters such as Factor and Offset, are then located in values of the <span class="Monospace">generation_parameters</span> property. The <span class="Monospace">sequence_representation</span> property specifies the LocalColumn type. The property can accept the following values:<br attr="ext"/><br attr="ext"/>
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
#------ Displaying local column size ---------
dd.MsgBoxDisp(oMyTargetLocalColumn.Size)
```

## See also

<div markdown="1">
<div class="SeeAlso"><p></p><table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>In implicit LocalColumns, you also can store the generation parameters in the values of the LocalColumn. The property <span class="Monospace">Size</span> then indicates how many generation parameters there are. Alternatively, the generation parameters can be stored in the <span class="Monospace">Generation_Parameters</span> property. In this case <span class="Monospace">Size</span> always returns the value 0.<br attr="ext"/>If the LocalColumns contain raw data, <span class="Monospace">Size</span> always returns the amount of the raw data in the Values vector. Parameters such as Factor and Offset, are then located in values of the <span class="Monospace">generation_parameters</span> property. The <span class="Monospace">sequence_representation</span> property specifies the LocalColumn type. The property can accept the following values:<br attr="ext"/><br attr="ext"/>
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
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Size_ITDMStoreElementWithBulk.htm`*
