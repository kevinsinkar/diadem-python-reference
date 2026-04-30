---
title: "ToActionObjButtonInt.GetBarID"
description: "Returns the name of the bar containing the bar element. You only can use this method in an event, such as OnClickCode . Use this method to define behavior for t"
---

# ToActionObjButtonInt.GetBarID

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: GetBarID for ActionObjButton

Returns the name of the bar containing the bar element. You only can use this method in an event, such as OnClickCode . Use this method to define behavior for this bar element in relation to the position of the bar element.

## Signature

```python
sGetBarID = Object.GetBarID
```

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyButton")) :
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton", "CustomButton")
    oMyActionObj.Picture = "favicon.ico"
    oMyActionObj.Tooltip = "MyButton"
    oMyActionObj.OnClickCode.Code = "Call MsgBoxDisp(\"MyButton\")"
else:
    oMyActionObj = dd.BarManager.ActionObjs("MyButton")
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oMyActionObj)

oMyActionObj.OnClickCode.Code            ="Select Case LCase(This.GetBarID)"
oMyActionObj.OnClickCode.AddCodeLine("Case \"navmain\"")
oMyActionObj.OnClickCode.AddCodeLine(" Call print(\"Code for NAVIGATOR\")")
oMyActionObj.OnClickCode.AddCodeLine("Case \"viewmain\"")
oMyActionObj.OnClickCode.AddCodeLine("Call print(\"Code for VIEW\")")
oMyActionObj.OnClickCode.AddCodeLine("Case \"anamain\"")
oMyActionObj.OnClickCode.AddCodeLine("Call print(\"Code for ANALYSIS\")")
oMyActionObj.OnClickCode.AddCodeLine("Case \"repmain\"")
oMyActionObj.OnClickCode.AddCodeLine("Call print(\"Code for REPORT\")")
oMyActionObj.OnClickCode.AddCodeLine("Case \"dacmain\"")
oMyActionObj.OnClickCode.AddCodeLine("Call print(\"Code for DAC\")")
oMyActionObj.OnClickCode.AddCodeLine("Case \"viscmain\"")
oMyActionObj.OnClickCode.AddCodeLine("Call print(\"Code for VISUAL\")")
oMyActionObj.OnClickCode.AddCodeLine("Case \"scrmain\"")
oMyActionObj.OnClickCode.AddCodeLine("Call print(\"Code for SCRIPT\")")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_GetBarID_ToActionObjButtonInt.htm`*
