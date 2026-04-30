---
title: "ToBarInt.ActionObjPictureWidth"
description: "Specifies the width of the graphics that DIAdem displays on the elements of a bar, in pixels. This way, the property ensures the uniform appearance of the bar. "
---

# ToBarInt.ActionObjPictureWidth

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: ActionObjPictureWidth for Bar

Specifies the width of the graphics that DIAdem displays on the elements of a bar, in pixels. This way, the property ensures the uniform appearance of the bar. The specifications ActionObjPictureWidth and ActionObjPictureHeight refer to a screen resolution of 96 DPI. With other screen resolutions, DIAdem either scales the graphic or uses a matching symbol size from the ICO file. For example, if the resolution is 44 DPI, DIAdem scales the graphic by 150% or uses a 24 pixel-sized symbol, if that is available in the ICO file, for 16 pixel-sized specifications.

## Signature

```python
obj.ActionObjPictureWidth
```

## Python example

```python
sgBarId = "MyBar"
if (not dd.BarManager.Bars.Exists(sgBarId)) :
    dd.BarManager.Bars.Add(sgBarId)
    dd.BarManager.Bars(sgBarId).ActionObjPictureWidth = 16
    dd.BarManager.Bars(sgBarId).ActionObjPictureHeight = 16
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../tobarint-actionobjpictureheight/">ActionObjPictureHeight</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_ActionObjPictureWidth_ToBarInt.htm`*
