---
title: "IToPythonGraphicInt.ToolbarVisible"
description: "Specifies whether the toolbar is visible in a Python graphic display in DIAdem VIEW."
---

# IToPythonGraphicInt.ToolbarVisible

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ToolbarVisible for PythonGraphic

Specifies whether the toolbar is visible in a Python graphic display in DIAdem VIEW.

## Signature

```python
obj.ToolbarVisible
```

## Python example

```python
PyGraphic = dd.View.ActiveSheet.ActiveArea.DisplayObj
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "PythonGraphic" :
    PyGraphic.ToolbarVisible = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="#" data-unresolved="1">Python Graphic</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Spectrograph in VIEW with the Python Graphic</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ToolbarVisible_IToPythonGraphicInt.htm`*
