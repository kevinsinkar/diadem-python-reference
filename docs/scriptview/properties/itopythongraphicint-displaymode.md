---
title: "IToPythonGraphicInt.DisplayMode"
description: "Determines how the aspect ratio and size of the graphic should affect the image display. The graphic to be displayed can be displayed maintaining its aspect rat"
---

# IToPythonGraphicInt.DisplayMode

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DisplayMode for PythonGraphic

Determines how the aspect ratio and size of the graphic should affect the image display. The graphic to be displayed can be displayed maintaining its aspect ratio or completely filling the area without a border. If the aspect ratio of the graphic is taken into account, the graphic can either always be enlarged or reduced to fit within the area, or it can be displayed in its original size, which means that no enlargement takes place. The graphic is always displayed centered in the area. Tip Create your graphic with the dimensions of the VIEW area so that the graphic does not enlarge or shrink, thus avoiding losses in the image display. How to calculate the appropriate size for your graphic can be found in the script template for a Python graphic in the description of the ON_CURSORCHANGED_SCRIPTGRAPHIC function or on the help page for the Python script of the Python graphic.

## Signature

```python
obj.DisplayMode
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Tip</strong> Create your graphic with the dimensions of the VIEW area so that the graphic does not enlarge or shrink, thus avoiding losses in the image display. How to calculate the appropriate size for your graphic can be found in the script template for a Python graphic in the description of the <a href="#" data-unresolved="1">ON_CURSORCHANGED_SCRIPTGRAPHIC</a> function or on the <a href="#" data-unresolved="1">help page for the Python script</a> of the Python graphic.</td></tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eVIEWDisplayModeFullSized` | 1 | Reduce or enlarge the graphic while maintaining the aspect ratio. |
| `eVIEWDisplayModeSized` | 2 | Reduce the graphic or display it at its original size, while maintaining the aspect ratio. |
| `eVIEWDisplayModeStretch` | 3 | Resize the graphic to fill the area completely. |

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "PythonGraphic"
PyGraphic = dd.View.Sheets(1).Areas(1).DisplayObj
PyGraphic.DisplayMode = dd.eVIEWDisplayModeStretch
dd.WndShow("VIEW")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="#" data-unresolved="1">Python Graphic</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Spectrograph in VIEW with the Python Graphic</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DisplayMode_IToPythonGraphicInt.htm`*
