---
title: "ToActionObjPopupInt.BarID"
description: "Specifies the name of the bar that DIAdem opens when the button is clicked."
---

# ToActionObjPopupInt.BarID

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: BarID for ActionObjPopup

Specifies the name of the bar that DIAdem opens when the button is clicked.

## Signature

```python
obj.BarID
```

## Python example

```python
oFFTBar = dd.BarManager.Bars.Add("MyFFTBar")

oActionObj = dd.BarManager.ActionObjs.Add("FFTPopup","CustomPopup")
oActionObj.BarID = oFFTBar.ID
dd.BarManager.Bars("ANAGroup").UsedActionObjs.Add(oActionObj)

oActionObj = dd.BarManager.ActionObjs.Copy("AnaDlgChnFFT2","MyFFT")
oFFTBar.UsedActionObjs.Add(oActionObj)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_BarID_ToActionObjPopupInt.htm`*
