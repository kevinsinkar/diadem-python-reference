---
title: "ITDMBrowseSettings.RootEntity"
description: "Specifies in a data store the top entity of a browse path ."
---

# ITDMBrowseSettings.RootEntity

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: RootEntity for BrowseSettings

Specifies in a data store the top entity of a browse path .

## Signature

```python
return_value = obj.RootEntity
```

## Python example

```python
oMyBrowseSettings = dd.Navigator.Display.CurrDatastore.GetBrowseSettings()
oMyRootEntity = oMyBrowseSettings.RootEntity
print(oMyRootEntity.EntityType.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_RootEntity_ITDMBrowseSettings.htm`*
