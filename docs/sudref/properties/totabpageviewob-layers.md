---
title: "ToTabPageViewOb.Layers"
description: "Assigns the controls of a tab to different layers. Use this property to make the controls you assign to one layer visible or invisible while you generate or dis"
---

# ToTabPageViewOb.Layers

!!! abstract "Property &middot; `Sudref.chm`"
    Property: Layers for Page

Assigns the controls of a tab to different layers. Use this property to make the controls you assign to one layer visible or invisible while you generate or display the user dialog box. The property does not affect which control is on top.

## Signature

```python
obj.Layers(Name)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>The <span class="Monospace">Layername</span> method returns the name of the layer a control is in.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Page1.Layers("Layer1") = FALSE
```

---

*Source: `Sudref/properties/SUD_property_Layers_ToTabPageViewOb.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
