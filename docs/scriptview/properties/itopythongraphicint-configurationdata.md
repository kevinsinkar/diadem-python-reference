---
title: "IToPythonGraphicInt.ConfigurationData"
description: "Specifies optional configuration settings of the Python graphic area that are managed as text and stored in the layout. Within your Python script , you determin"
---

# IToPythonGraphicInt.ConfigurationData

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ConfigurationData for PythonGraphic

Specifies optional configuration settings of the Python graphic area that are managed as text and stored in the layout. Within your Python script , you determine what information about the Python graphic is stored and in what form. It can be just one piece of information or several, which you separate, for example, with semicolons or store in JSON format. The user of the Python graphic can change the configuration settings via the "Configure" button of the area's function bar if you have implemented, for example, an input dialog for the Python graphic in the Python script in the ON_CONFIGURE_SCRIPTGRAPHIC function.

## Signature

```python
obj.ConfigurationData
```

## Python example

```python
dd.View.LoadLayout("Example.TDV")
PyGraphicArea = dd.View.Sheets(1).Areas(1).SplitRight("PyArea", 0.5)
PyGraphicArea.DisplayObjType = "PythonGraphic"
PyGraphicArea.DisplayObj.ConfigurationData = "2"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="#" data-unresolved="1">Python Graphic</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Spectrograph in VIEW with the Python Graphic</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ConfigurationData_IToPythonGraphicInt.htm`*
