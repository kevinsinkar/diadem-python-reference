---
title: "ToActionObjButtonInt.Shape"
description: "Specifies how DIAdem displays a bar element in a bar. Note If a bar element is predefined, which means the Child property has the value eActObjKindPreset , this"
---

# ToActionObjButtonInt.Shape

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Shape for ActionObjButton

Specifies how DIAdem displays a bar element in a bar. Note If a bar element is predefined, which means the Child property has the value eActObjKindPreset , this property is write protected. If the bar element is user-defined ( Child =eActObjKindCustom ), you can change this property.

## Signature

```python
obj.Shape
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  If a bar element is predefined, which means the <a href="../toactionobjbuttonint-kind/">Child</a> property has the value <span class="Monospace">eActObjKindPreset</span>, this property is write protected. If the bar element is user-defined (<a href="../toactionobjbuttonint-kind/">Child</a><span class="Monospace">=eActObjKindCustom</span>), you can change this property.</td>
</tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eActObjShapeStandard` | 0 | DIAdem displays the bar element as a button. |
| `eActObjShapeTab` | 1 | DIAdem displays the bar element as a tab. |

## Python example

```python
dd.MsgBoxDisp("Shape of second element: " + dd.BarManager.Bars("DIAPanels").UsedActionObjs(2).Shape)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Shape_ToActionObjButtonInt.htm`*
