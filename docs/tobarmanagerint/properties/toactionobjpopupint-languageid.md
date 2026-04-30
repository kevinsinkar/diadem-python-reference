---
title: "ToActionObjPopupInt.LanguageId"
description: "Specifies the scripting language used for the OnRefreshCode event of the toolbar element. Possible values are \"VBS\" (VBScript) and \"PY\" (Python).  The default v"
---

# ToActionObjPopupInt.LanguageId

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: LanguageId for ActionObjPopup

Specifies the scripting language used for the OnRefreshCode event of the toolbar element. Possible values are "VBS" (VBScript) and "PY" (Python).  The default value is "VBS".

## Signature

```python
obj.LanguageId
```

## Python example

```python
oActionObj = dd.BarManager.ActionObjs("MyPopup")
oActionObj.LanguageId = "PY"
oActionObj.OnRefreshCode.Code = "this.Enable = (GlobUsedChn > 0)"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_LanguageId_ToActionObjPopupInt.htm`*
