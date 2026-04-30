---
title: "IProperty.Default"
description: "Specifies whether a property is a base property ."
---

# IProperty.Default

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Default for Property <DataPlugin>

Specifies whether a property is a base property .

## Signature

```python
obj.Default
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProp in Root.Properties:
    if not oMyProp.Default:
        oMyProp.Value = ""
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Default_IProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
