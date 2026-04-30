---
title: "ITDMBrowseEntity.ParentPath"
description: "Specifies in the browse path of a data store the reference to the superordinate entity."
---

# ITDMBrowseEntity.ParentPath

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ParentPath for BrowseEntity

Specifies in the browse path of a data store the reference to the superordinate entity.

## Signature

```python
obj.ParentPath
```

## Python example

```python
oMyElement = dd.Navigator.Display.CurrDatastore.Browser.FocusedElement
oMyBrowseSettings = dd.Navigator.Display.CurrDatastore.GetBrowseSettings()
oMyBrowseEntity = oMyBrowseSettings.GetBrowseEntity(oMyElement)
dd.MsgBoxDisp(oMyBrowseEntity.ParentPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ParentPath_ITDMBrowseEntity.htm`*
