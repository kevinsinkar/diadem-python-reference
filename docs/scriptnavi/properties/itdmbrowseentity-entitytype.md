---
title: "ITDMBrowseEntity.EntityType"
description: "Specifies in the browse path of a data store the type of an entity."
---

# ITDMBrowseEntity.EntityType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: EntityType for BrowseEntity

Specifies in the browse path of a data store the type of an entity.

## Signature

```python
return_value = obj.EntityType
```

## Python example

```python
oMyElement = dd.Navigator.Display.CurrDatastore.Browser.FocusedElement
oMyBrowseSettings = dd.Navigator.Display.CurrDatastore.GetBrowseSettings()
oMyBrowseEntity = oMyBrowseSettings.GetBrowseEntity(oMyElement)
dd.MsgBoxDisp(oMyBrowseEntity.EntityType.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_EntityType_ITDMBrowseEntity.htm`*
