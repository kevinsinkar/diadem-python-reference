---
title: "IToPythonGraphicInt.Area"
description: "Returns the area in DIAdem VIEW that contains a Python graphic display."
---

# IToPythonGraphicInt.Area

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Area for PythonGraphic

Returns the area in DIAdem VIEW that contains a Python graphic display.

## Signature

```python
return_value = obj.Area
```

## Python example

```python
PyGraphicArea = dd.View.Sheets(1).Areas(1).SplitRight("PyArea", 0.5)
PyGraphicArea.DisplayObjType = "PythonGraphic"
dd.WndShow("VIEW")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="#" data-unresolved="1">Python Graphic</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Spectrograph in VIEW with the Python Graphic</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Area_IToPythonGraphicInt.htm`*
