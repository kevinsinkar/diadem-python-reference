---
title: "ToActionObjButtonInt.Kind"
description: "Specifies whether the bar element is a predefined or a user-defined bar element."
---

# ToActionObjButtonInt.Kind

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Kind for ActionObjButton

Specifies whether the bar element is a predefined or a user-defined bar element.

## Signature

```python
obj.Kind
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>A predefined bar element has several specified properties some of which you cannot change, such as <span class="Monospace">OnClickCode</span>. You can configure all properties of a user-defined bar element.</td>
</tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eActObjKindPreset` | 0 | Predefined bar element |
| `eActObjKindCustom` | 1 | Free bar element |

## Python example

```python
oMyObject = dd.BarManager.ActionObjs("MyButton")
if (oMyObject.Kind == dd.eActObjKindCustom) :
    oMyObject.OnClickCode.Code ="Call MsgBoxDisp(\"Hello\")"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Kind_ToActionObjButtonInt.htm`*
