---
title: "ITDMBrowseEntity.ChildPath"
description: "Specifies in the browse path of a data store the reference to the subordinate entity."
---

# ITDMBrowseEntity.ChildPath

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ChildPath for BrowseEntity

Specifies in the browse path of a data store the reference to the subordinate entity.

## Signature

```python
obj.ChildPath
```

## Python example

```python
oMyElement = dd.Navigator.Display.CurrDatastore.Browser.FocusedElement
oMyBrowseSettings = dd.Navigator.Display.CurrDatastore.GetBrowseSettings()
oMyBrowseEntity = oMyBrowseSettings.GetBrowseEntity(oMyElement)
dd.MsgBoxDisp(oMyBrowseEntity.ChildPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ChildPath_ITDMBrowseEntity.htm`*
