---
title: "ToActionObjCheckInt.GetBarID"
description: "Returns the name of the bar that contains the bar element. You only can use this method in an event, such as OnClickCode . Use this method to define behavior fo"
---

# ToActionObjCheckInt.GetBarID

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: GetBarID for ActionObjCheckbutton

Returns the name of the bar that contains the bar element. You only can use this method in an event, such as OnClickCode . Use this method to define behavior for this bar element in relation to the position of the bar element.

## Signature

```python
sGetBarID = Object.GetBarID
```

## Python example

```python
oMyObj = dd.BarManager.ActionObjs("MyCheckButton")
oMyObj.OnRefreshCode.Code = "If This.GetBarID = \"SCRMain\" then"
oMyObj.OnRefreshCode.AddCodeLine(" This.Enable = (GlobUsedChn > 0)")
oMyObj.OnRefreshCode.AddCodeLine("This.Check = PtlShow")

oMyObj.OnClickCode.Code = "PtlShow = not This.Check"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_GetBarID_ToActionObjCheckInt.htm`*
