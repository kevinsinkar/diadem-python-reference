---
title: "IProperty.Name"
description: "Returns the name of a Property object."
---

# IProperty.Name

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Name for Property <DataPlugin>

Returns the name of a Property object.

## Signature

```python
obj.Name
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProp in Root.Properties:
    if oMyProp.Name == "Sensor_Type":
        bfound = TRUE
if not bFound:
    Root.Properties.Add("Sensor_type","TC-N")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Name_IProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
