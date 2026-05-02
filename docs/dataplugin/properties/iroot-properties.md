---
title: "IRoot.Properties"
description: "Contains the Properties collection associated with a Root object."
---

# IRoot.Properties

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Properties for Root <DataPlugin>

Contains the Properties collection associated with a Root object.

## Signature

```python
return_value = obj.Properties
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
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Properties_IRoot.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
