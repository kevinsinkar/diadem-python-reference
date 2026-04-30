---
title: "ToBarInt"
description: "The Bar object provides a bar that you can use in DIAdem."
---

# ToBarInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: Bar

The Bar object provides a bar that you can use in DIAdem.

## Python example

```python
objs = []
bar = dd.BarManager.Bars(1)
for obj in bar.UsedActionObjs:
    objs.append(obj.ID)
print("Bar:", bar.ID, objs)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tobarint-actionobjpictureheight/">ActionObjPictureHeight</a> | <a href="../../properties/tobarint-actionobjpicturewidth/">ActionObjPictureWidth</a> | <a href="../../properties/tobarint-id/">ID</a> | <a href="../../properties/tobarint-position/">Position</a> | <a href="../../properties/tobarint-style/">Style</a> | <a href="../../properties/tobarint-usedactionobjs/">UsedActionObjs</a> | <a href="../../properties/tobarint-visible/">Visible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tobarint-refresh/">Refresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../tobarmanageruiint/">BarManager</a>.<a href="../../methods/tobarmanageruiint-addmenubar/">AddMenuBar</a> | 
<a href="../tobarmanagerint/">BarManagerUnattached</a>.<a href="../../methods/tobarmanagerint-addmenubar/">AddMenuBar</a> | 
<a href="../../collections/bars/">Bars</a>.<a href="../../methods/tobarlistint-add/">Add</a> | 
<a href="../../collections/bars/">Bars</a>.<a href="../../methods/tobarlistint-item/">Item</a> | 
<a href="../../collections/usedbars/">UsedBars</a>.<a href="../../methods/tousedbarlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToBarInt.htm`*
