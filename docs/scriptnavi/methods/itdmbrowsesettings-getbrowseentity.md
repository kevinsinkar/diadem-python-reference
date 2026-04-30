---
title: "ITDMBrowseSettings.GetBrowseEntity"
description: "Determines in a data store the entity of an element from the browse path ."
---

# ITDMBrowseSettings.GetBrowseEntity

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetBrowseEntity for BrowseSettings

Determines in a data store the entity of an element from the browse path .

## Signature

```python
return_value = obj.GetBrowseEntity(Element)
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

*Source: `ScriptNavi/methods/navigator_method_GetBrowseEntity_ITDMBrowseSettings.htm`*
