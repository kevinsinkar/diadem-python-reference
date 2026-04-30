---
title: "ToActionObjButtonInt"
description: "The ActionObjButton object provides a bar element that corresponds to a button. The element is a button if the Type property of the bar element contains the val"
---

# ToActionObjButtonInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: ActionObjButton

The ActionObjButton object provides a bar element that corresponds to a button. The element is a button if the Type property of the bar element contains the value eActObjTypeButton .

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyButton")) :
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton", "CustomButton")
    oMyActionObj.Picture = "favicon.ico"
    oMyActionObj.Tooltip = "MyButton"
    oMyActionObj.OnClickCode.Code = "Call MsgBoxDisp(\"MyButton\")"
else:
    oMyActionObj = dd.BarManager.ActionObjs("MyButton")
dd.BarManager.Bars("ANAMain").UsedActionObjs.Add(oMyActionObj)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/toactionobjbuttonint-baseid/">BaseID</a> | <a href="../../properties/toactionobjbuttonint-caption/">Caption</a> | <a href="../../properties/toactionobjbuttonint-enable/">Enable</a> | <a href="../../properties/toactionobjbuttonint-id/">ID</a> | <a href="../../properties/toactionobjbuttonint-kind/">Kind</a> | <a href="../../properties/toactionobjbuttonint-languageid/">LanguageId</a> | <a href="../../properties/toactionobjbuttonint-onclickcode/">OnClickCode</a> | <a href="../../properties/toactionobjbuttonint-onrefreshcode/">OnRefreshCode</a> | <a href="../../properties/toactionobjbuttonint-picture/">Picture</a> | <a href="../../properties/toactionobjbuttonint-shape/">Shape</a> | <a href="../../properties/toactionobjbuttonint-tooltip/">Tooltip</a> | <a href="../../properties/toactionobjbuttonint-type/">Type</a> | <a href="../../properties/toactionobjbuttonint-visible/">Visible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/toactionobjbuttonint-getbarid/">GetBarID</a> | <a href="../../methods/toactionobjbuttonint-reset/">Reset</a> | <a href="../../methods/toactionobjbuttonint-resetcaption/">ResetCaption</a> | <a href="../../methods/toactionobjbuttonint-resetpicture/">ResetPicture</a> | <a href="../../methods/toactionobjbuttonint-resettooltip/">ResetTooltip</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-add/">Add</a> | <a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-copy/">Copy</a> | <a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-item/">Item</a> | <a href="../tobarmanageruiint/">BarManager</a>.<a href="../../methods/tobarmanageruiint-addmenuitem/">AddMenuItem</a> | <a href="../tobarmanagerint/">BarManagerUnattached</a>.<a href="../../methods/tobarmanagerint-addmenuitem/">AddMenuItem</a> | <a href="../../collections/usedactionobjs/">UsedActionObjs</a>.<a href="../../methods/tousedactionobjlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToActionObjButtonInt.htm`*
