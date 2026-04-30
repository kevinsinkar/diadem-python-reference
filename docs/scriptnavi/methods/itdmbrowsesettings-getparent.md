---
title: "ITDMBrowseSettings.GetParent"
description: "Determines the superordinate element of an element in the browse path ."
---

# ITDMBrowseSettings.GetParent

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetParent for BrowseSettings

Determines the superordinate element of an element in the browse path .

## Signature

```python
return_value = obj.GetParent(Element)
```

## Python example

```python
oMyElement = dd.Navigator.Display.CurrDatastore.Browser.FocusedElement
oMyBrowseSettings = dd.Navigator.Display.CurrDatastore.GetBrowseSettings()
oMyParent = oMyBrowseSettings.GetParent(oMyElement)
dd.MsgBoxDisp("Name: " + oMyParent.Name + "\r\n" + "Type: " + oMyParent.Type)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetParent_ITDMBrowseSettings.htm`*
