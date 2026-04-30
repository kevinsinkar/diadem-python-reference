---
title: "ToActionObjCheckInt"
description: "The ActionObjCheckbutton object provides a bar element that corresponds to a button that displays a status. When the Type property of the bar element contains t"
---

# ToActionObjCheckInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: ActionObjCheckbutton

The ActionObjCheckbutton object provides a bar element that corresponds to a button that displays a status. When the Type property of the bar element contains the value eActObjTypeCheckButton , the element is a button that displays the status.

## Python example

```python
oFloating = dd.BarManager.ActionObjs.Add("PtlFloatingOnOff", "CustomCheckButton")
oFloating.Tooltip = "Floating Portal"
oFloating.OnRefreshCode.Code = "This.Check = PtlFloating"
oFloating.OnClickCode.Code = "PtlFloating = not This.Check"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oFloating)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/toactionobjcheckint-baseid/">BaseID</a> | <a href="../../properties/toactionobjcheckint-check/">Caption</a> | <a href="../../properties/toactionobjcheckint-check/">Check</a> | <a href="../../properties/toactionobjcheckint-enable/">Enable</a> | <a href="../../properties/toactionobjcheckint-id/">ID</a> | <a href="../../properties/toactionobjcheckint-kind/">Kind</a> | <a href="../../properties/toactionobjcheckint-languageid/">LanguageId</a> | <a href="../../properties/toactionobjcheckint-onclickcode/">OnClickCode</a> | <a href="../../properties/toactionobjcheckint-onrefreshcode/">OnRefreshCode</a> | <a href="../../properties/toactionobjcheckint-picture/">Picture</a> | <a href="../../properties/toactionobjcheckint-shape/">Shape</a> | <a href="../../properties/toactionobjcheckint-tooltip/">Tooltip</a> | <a href="../../properties/toactionobjcheckint-type/">Type</a> | <a href="../../properties/toactionobjcheckint-visible/">Visible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/toactionobjcheckint-getbarid/">GetBarID</a> | <a href="../../methods/toactionobjcheckint-reset/">Reset</a> | <a href="../../methods/toactionobjcheckint-resetcaption/">ResetCaption</a> | <a href="../../methods/toactionobjcheckint-resetpicture/">ResetPicture</a> | <a href="../../methods/toactionobjcheckint-resettooltip/">ResetTooltip</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-add/">Add</a> | <a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-copy/">Copy</a> | <a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-item/">Item</a> | <a href="../../collections/usedactionobjs/">UsedActionObjs</a>.<a href="../../methods/tousedactionobjlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToActionObjCheckInt.htm`*
