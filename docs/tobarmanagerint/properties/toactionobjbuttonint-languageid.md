---
title: "ToActionObjButtonInt.LanguageId"
description: "Specifies the scripting language used for the OnClickCode and OnRefreshCode events of the bar element. Possible values are \"VBS\" (VBScript) and \"PY\" (Python). T"
---

# ToActionObjButtonInt.LanguageId

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: LanguageId for ActionObjButton

Specifies the scripting language used for the OnClickCode and OnRefreshCode events of the bar element. Possible values are "VBS" (VBScript) and "PY" (Python). The default value is "VBS" .

## Signature

```python
obj.LanguageId
```

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyButton")):
  oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton", "CustomButton")
  oMyActionObj.LanguageId = "PY"
  oMyActionObj.OnClickCode.Code = "dd.Data.Root.Clear()"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oMyActionObj)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_LanguageId_ToActionObjButtonInt.htm`*
