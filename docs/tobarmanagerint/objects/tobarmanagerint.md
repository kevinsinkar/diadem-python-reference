---
title: "ToBarManagerInt"
description: "Use the BarManagerUnattached object to access the panels, the bars, and the bar elements of an additional bar definition, which you can create, load, and save i"
---

# ToBarManagerInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: BarManagerUnattached

Use the BarManagerUnattached object to access the panels, the bars, and the bar elements of an additional bar definition, which you can create, load, and save independently of the DIAdem interface. Changes to the BarManagerUnattached object do not impact the visible bars.

## Python example

```python
oMyBardef = dd.BarManager.Create("")
oMyActionObj = dd.BarManager.ActionObjs.Add("MyObjPopup", "CustomPopUp")
oMyActionObj.Tooltip = "Opens ANAMain"
oMyActionObj.BarID   = "ANAMain"
dd.BarManager.Bars("SCRGroup").UsedActionObjs.Add(oMyActionObj)
dd.BarManager.SaveAsDeployment("MyBarDef.bdy")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tobarmanagerint-actionobjs/">ActionObjs</a> | <a href="../../properties/tobarmanagerint-bars/">Bars</a> |<a href="../../properties/tobarmanagerint-dataportal/">DataPortal</a> | <a href="../../properties/tobarmanagerint-filename/">FileName</a> | <a href="../../properties/tobarmanagerint-filepath/">FilePath</a> | <a href="../../properties/tobarmanagerint-panels/">Panels</a> | <a href="../../properties/tobarmanagerint-resourcepath/">ResourcePath</a> | <a href="../../properties/tobarmanagerint-shell/">Shell</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tobarmanagerint-create/">Create</a> | <a href="../../methods/tobarmanagerint-createfromdeployment/">CreateFromDeployment</a> | <a href="../../methods/tobarmanagerint-import/">Import</a> | <a href="../../methods/tobarmanagerint-ismodified/">IsModified</a> | <a href="../../methods/tobarmanagerint-load/">Load</a> | <a href="../../methods/tobarmanagerint-reset/">Reset</a> | <a href="../../methods/tobarmanagerint-save/">Save</a> | <a href="../../methods/tobarmanagerint-saveasdeployment/">SaveAsDeployment</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../tobarmanageruiint/">BarManager</a>.<a href="../../methods/tobarmanageruiint-create/">Create</a> | <a href="../tobarmanageruiint/">BarManager</a>.<a href="../../methods/tobarmanageruiint-createfromdeployment/">CreateFromDeployment</a> | <a href="./">BarManagerUnattached</a>.<a href="../../methods/tobarmanagerint-create/">Create</a> | <a href="./">BarManagerUnattached</a>.<a href="../../methods/tobarmanagerint-createfromdeployment/">CreateFromDeployment</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToBarManagerInt.htm`*
