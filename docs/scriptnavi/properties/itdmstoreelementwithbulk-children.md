---
title: "ITDMStoreElementWithBulk.Children"
description: "Returns the subordinate elements of a data element in a data store. Use the Children property to navigate from the root element to the measurement quantities."
---

# ITDMStoreElementWithBulk.Children

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Children for ElementWithValues <DataStore>

Returns the subordinate elements of a data element in a data store. Use the Children property to navigate from the root element to the measurement quantities.

## Signature

```python
return_value = obj.Children
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Children_ITDMStoreElementWithBulk.htm`*
