---
title: "ITDMBrowseEntity.ChildEntity"
description: "Specifies in the browse path of a data store the entity located below a given entity."
---

# ITDMBrowseEntity.ChildEntity

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ChildEntity for BrowseEntity

Specifies in the browse path of a data store the entity located below a given entity.

## Signature

```python
return_value = obj.ChildEntity
```

## Python example

```python
oMyElement = dd.Navigator.Display.CurrDatastore.Browser.FocusedElement
oMyBrowseSettings = dd.Navigator.Display.CurrDatastore.GetBrowseSettings()
oMyBrowseEntity = oMyBrowseSettings.GetBrowseEntity(oMyElement)
dd.MsgBoxDisp(oMyBrowseEntity.ChildEntity.EntityType.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ChildEntity_ITDMBrowseEntity.htm`*
