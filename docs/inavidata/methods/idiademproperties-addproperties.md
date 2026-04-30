---
title: "IDiademProperties.AddProperties"
description: "Adds copies of existing properties to the properties of an element (root, channel group, or channel), in the script interface for internal data."
---

# IDiademProperties.AddProperties

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddProperties for Properties <Data>

Adds copies of existing properties to the properties of an element (root, channel group, or channel), in the script interface for internal data.

## Signature

```python
obj.AddProperties(Properties, Prefix)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If the property with the specified name exists, DIAdem does not overwrite this property but retains the original property including its value.</td></tr></table>
</div>

## Python example

```python
oMyProperties = dd.Data.Root.ChannelGroups(1).Properties
oMyChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyChannel.Properties.AddProperties(oMyProperties)
```

```python
oMySource = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyDestination = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyDestination.Properties.AddProperties(oMySource)
```

```python
oMySourceProperties      = dd.Data.Root.ChannelGroups(1).Properties
oMyDestinationChn        = dd.Data.Root.ChannelGroups(2).Channels(1)
AddOverwriteProperties(oMySourceProperties, oMyDestinationChn)

def AddOverwriteProperties(oSourceProperties, oDestinationChn):
    oDestinationProperties = oDestinationChn.Properties
    for oProperty in oSourceProperties:
        PropertyName = oProperty.Name
        if oDestinationProperties.Exists(PropertyName) :
            if (oProperty.DataType == oDestinationProperties(PropertyName).DataType) :
                oDestinationProperties.Add(oProperty.Name, oProperty.Value)
            else:
                print ("Please change the datatype of the property: " , PropertyName)
        else:
            oDestinationProperties.Add(oProperty.Name, oProperty.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddProperties_IDiademProperties.htm`*
