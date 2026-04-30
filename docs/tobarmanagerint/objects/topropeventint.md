---
title: "ToPropEventInt"
description: "The Event object provides VBS code that is executed at a specific point in time, for example, when a bar element is clicked. Within the VBS code you can use and"
---

# ToPropEventInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: Event

The Event object provides VBS code that is executed at a specific point in time, for example, when a bar element is clicked. Within the VBS code you can use and change the properties of the bar element. Use the This variable to access the bar element. You can access the VBS code only under certain conditions.

## Notes

<div markdown="1">
<table class="Borderless" id="table6">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Do not implement your own <span class="Monospace">Function</span> or <span class="Monospace">Sub</span> procedure within the VBS code.</td>
</tr>
</table>
<table class="Borderless" id="table7">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must not specify <span class="Monospace">Option Explicit</span> in the VBS code because DIAdem sets this statement implicitly.</td>
</tr>
</table>
</div>

## Python example

```python
oActionObj = dd.BarManager.ActionObjs("MyButton")
oActionObj.OnRefreshCode.Code = "This.Enable = (GlobUsedChn > 0)"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/topropeventint-code/">Code</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/topropeventint-addcodeline/">AddCodeLine</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../toactionobjbuttonint/">ActionObjButton</a>.<a href="../../properties/toactionobjbuttonint-onclickcode/">OnClickCode</a> | <a href="../toactionobjbuttonint/">ActionObjButton</a>.<a href="../../properties/toactionobjbuttonint-onrefreshcode/">OnRefreshCode</a> | <a href="../toactionobjcheckint/">ActionObjCheckbutton</a>.<a href="../../properties/toactionobjcheckint-onclickcode/">OnClickCode</a> | <a href="../toactionobjcheckint/">ActionObjCheckbutton</a>.<a href="../../properties/toactionobjcheckint-onrefreshcode/">OnRefreshCode</a> | <a href="../toactionobjpopupint/">ActionObjPopup</a>.<a href="../../properties/toactionobjpopupint-onrefreshcode/">OnRefreshCode</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToPropEventInt.htm`*
