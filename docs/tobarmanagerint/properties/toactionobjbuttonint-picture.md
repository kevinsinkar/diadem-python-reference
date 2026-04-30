---
title: "ToActionObjButtonInt.Picture"
description: "Specifies which graphic appears for the button on the DIAdem interface. For DIAdem to display a graphic, the graphics file must contain a symbol that is same si"
---

# ToActionObjButtonInt.Picture

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Picture for ActionObjButton

Specifies which graphic appears for the button on the DIAdem interface. For DIAdem to display a graphic, the graphics file must contain a symbol that is same size as the properties ActionObjPictureHeight and ActionObjPictureWidth of the bar that is to contain the symbol. DIAdem uses 16*16 pixels as the default symbol size for the toolbar and 32*32 pixels for the group bar.

## Signature

```python
return_value = obj.Picture
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Specify the name of the ICO file without a path. DIAdem receives user-defined IOC files in the <a href="../tobarmanagerint-resourcepath/">Resource folder</a>. </td>
</tr>
</table>
</div>

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyObjButton")) :
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyObjButton", "CustomButton")
    oMyActionObj.Picture = "favicon.ico"
    oMyActionObj.Tooltip = "MyObjButton"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oMyActionObj)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Picture_ToActionObjButtonInt.htm`*
