---
title: "ToPropEventInt.AddCodeLine"
description: "Adds a line with VBS code to the Event object."
---

# ToPropEventInt.AddCodeLine

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: AddCodeLine for Event

Adds a line with VBS code to the Event object.

## Signature

```python
obj.AddCodeLine(Line)
```

## Python example

```python
oActionObj = dd.BarManager.ActionObjs.Add("MyButton","CustomButton")
oActionObj.OnClickCode.Code = "Dim MyVal"
oActionObj.OnClickCode.AddCodeLine("MyVal = dd.InputBoxDisp(\"Please enter value\")")
oActionObj.OnClickCode.AddCodeLine("Call MsgBoxDisp(\"Square of \" +MyVal+ \" : \"+ MyVal^2)")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_AddCodeLine_ToPropEventInt.htm`*
