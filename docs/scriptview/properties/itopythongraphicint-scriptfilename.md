---
title: "IToPythonGraphicInt.ScriptFileName"
description: "Specifies the file name for the Python script to be executed, which reacts to cursor movements and creates a graphic in the VIEW area. You can specify the file "
---

# IToPythonGraphicInt.ScriptFileName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ScriptFileName for PythonGraphic

Specifies the file name for the Python script to be executed, which reacts to cursor movements and creates a graphic in the VIEW area. You can specify the file name with or without an absolute path. If you do not specify a path, DIAdem searches for the Python file in the SCRIPT user folder. If ScriptFileName does not contain a filename, DIAdem uses a sample script to illustrate how the Python graphic works. Tip You can use path variables in the file name by adding a Path variable with two at signs as an expression : @@LayoutReadPath@@MyProject\MyScript.py .

## Signature

```python
obj.ScriptFileName
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Tip</strong> You can use path variables in the file name by adding a <a href="#" data-unresolved="1">Path variable with two at signs as an expression</a>: <span class="Monospace">@@LayoutReadPath@@MyProject\MyScript.py</span>.</td></tr>
</table>
</div>

## Python example

```python
PyGraphicArea = dd.View.Sheets(1).Areas(1).SplitRight("PyArea", 0.5)
PyGraphicArea.DisplayObjType = "PythonGraphic"
PyGraphicArea.DisplayObj.ScriptFileName = "@@LayoutReadPath@@CreateMyGraphic.py"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="#" data-unresolved="1">Python Graphic</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Spectrograph in VIEW with the Python Graphic</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ScriptFileName_IToPythonGraphicInt.htm`*
