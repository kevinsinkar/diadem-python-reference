---
title: "IToPythonGraphicInt.ShowSettingsDlg"
description: "Opens the dialog where you can specify the Python script to be used and make further settings for the configuration and display of the graphic."
---

# IToPythonGraphicInt.ShowSettingsDlg

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: ShowSettingsDlg for PythonGraphic

Opens the dialog where you can specify the Python script to be used and make further settings for the configuration and display of the graphic.

## Signature

```python
obj.ShowSettingsDlg()
```

## Python example

```python
PyGraphicArea = dd.View.Sheets(1).Areas(1).SplitRight("PyArea", 0.5)
PyGraphicArea.DisplayObjType = "PythonGraphic"
PyGraphicArea.DisplayObj.ShowSettingsDlg()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="#" data-unresolved="1">Python Graphic</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Spectrograph in VIEW with the Python Graphic</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_ShowSettingsDlg_IToPythonGraphicInt.htm`*
