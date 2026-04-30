---
title: "IPropertyHandling.ImportSet"
description: "Accepts a Loading Configuration for an ASAM data store. The load configuration specifies, which properties of an ASAM data store DIAdem imports when also loadin"
---

# IPropertyHandling.ImportSet

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ImportSet for PropertyHandling <Navigator>

Accepts a Loading Configuration for an ASAM data store. The load configuration specifies, which properties of an ASAM data store DIAdem imports when also loading the mass data into the Data Portal.

## Signature

```python
return_value = obj.ImportSet
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong> If you assign the value <span class="Monospace">Nothing</span> to the <span class="Monospace">ImportSet</span> parameter, DIAdem creates the standard browse setting for the open data store (Test/SubTest - Measurement - MeasurementQuantity), generates a minimum loading configuration, and then only transfers the name, the unit, and the description of each element into the Data Portal.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you do not assign a value to the <span class="Monospace">ImportSet</span> parameter, the associated command uses a standard loading configuration that is independent from the Browse settings.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you have specified a load configuration for the third parameter in the <a href="../../methods/inavigator-loaddata/">LoadData</a> command, this load configuration overwrites the load configuration in the <span class="Monospace">ImportParameter</span>.<span class="Monospace">PropertyHandling</span>.<span class="Monospace">ImportSet</span> object.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Clear()
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oMySelection = dd.Navigator.Display.CurrDataStore.Browser.SelectedElements
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")
oMyPropertyImportSet = dd.Navigator.Display.CurrDataStore.PropertyImportSet
oMyPropertyImportSet.Reset()
oMyPropertyImportSet.NamingSchema    = dd.eNamingSchemaTypeNamePropertyName
oMyPropertyImportSet.InheritanceMode = dd.eInheritanceCopyToChannelLevel
oMyImportParameter.PropertyHandling.ImportSet = oMyPropertyImportSet
oLoadedData = dd.Navigator.LoadData(oMySelection, oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ImportSet_IPropertyHandling.htm`*
