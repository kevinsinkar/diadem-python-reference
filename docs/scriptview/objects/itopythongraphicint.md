---
title: "IToPythonGraphicInt"
description: "The PythonGraphic object provides a Python graphic. Using a Python script that is assigned to the area, a graphic can be generated depending on the cursor movem"
---

# IToPythonGraphicInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: PythonGraphic

The PythonGraphic object provides a Python graphic. Using a Python script that is assigned to the area, a graphic can be generated depending on the cursor movement, which contains any graphic representation of the data using a Python library or an image export of a REPORT layout.

## Python example

```python
PyGraphicArea = dd.View.Sheets(1).Areas(1).SplitRight("PyArea", 0.5)
PyGraphicArea.DisplayObjType = "PythonGraphic"
PyGraphicArea.DisplayObj.ShowSettingsDlg()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itopythongraphicint-area/">Area</a> | <a href="../../properties/itopythongraphicint-configurationdata/">ConfigurationData</a> | <a href="../../properties/itopythongraphicint-displaymode/">DisplayMode</a> | <a href="../../properties/itopythongraphicint-scriptfilename/">ScriptFileName</a> | <a href="../../properties/itopythongraphicint-toolbarvisible/">ToolbarVisible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itopythongraphicint-showsettingsdlg/">ShowSettingsDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itoareaobjectint/">Area</a>.<a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="#" data-unresolved="1">Python Graphic</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Spectrograph in VIEW with the Python Graphic</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToPythonGraphicInt.htm`*
