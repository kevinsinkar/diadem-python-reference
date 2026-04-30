---
title: "IProperty"
description: "The Property object provides a property for the Root object, for the ChannelGroup object, or for the Channel object. This property is either a base property of "
---

# IProperty

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Property <DataPlugin>

The Property object provides a property for the Root object, for the ChannelGroup object, or for the Channel object. This property is either a base property of the data model, or a user-defined custom property.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProp in Root.Properties:
    if oMyProp.Name = "Sensor_Type":
        bfound = TRUE
if not bFound:
    Root.Properties.Add("Sensor_type","TC-N")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iproperty-datatype/">DataType</a> | <a href="../../properties/iproperty-default/">Default</a> | <a href="../../properties/iproperty-name/">Name</a> | <a href="../../properties/iproperty-size/">Size</a> | <a href="../../properties/iproperty-value/">Value</a> | <a href="../../properties/iproperty-values/">Values</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/properties/">Properties &lt;DataPlugin&gt;</a>.<a href="../../methods/iproperties-add/">Add</a> | <a href="../../collections/properties/">Properties &lt;DataPlugin&gt;</a>.<a href="../../methods/iproperties-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Store Object Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
