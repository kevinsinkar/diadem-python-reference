---
title: "IPropertyHandling.NameMappingFile"
description: "Specifies the name of a Technical Property Identifier Mapping file ( *.TPIM ). You are using TPIM files to replace the property identifiers."
---

# IPropertyHandling.NameMappingFile

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: NameMappingFile for PropertyHandling <Navigator>

Specifies the name of a Technical Property Identifier Mapping file ( *.TPIM ). You are using TPIM files to replace the property identifiers.

## Signature

```python
obj.NameMappingFile
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To create and save a TPIM file in DIAdem, select <strong>Settings»SystemLink TDM Server»Data Preparation</strong>, enable <strong>Replace property identifiers</strong>, click <strong>Edit</strong>, define the mapping rules and then click the <strong>Export Mapping</strong> button.</td></tr></table>
</div>

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")

oMyPropertyHandling = oMyImportParameter.PropertyHandling
oMyPropertyHandling.AutoUpdateChnCharacteristics = True
oMyPropertyHandling.InheritanceMode = dd.ePropInheritanceCopyToChannelLevel
oMyPropertyHandling.InheritanceSeparator = dd.ePropInheritanceSeparatorTilde
oMyPropertyHandling.NamingSchema = dd.ePropNamingSchemaPropertyName
oMyPropertyHandling.NameMappingFile = "D:\\test.tpim"
oMyPropertyHandling.ValueMappingFile = "D:\\test.tpvm"

dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_NameMappingFile_IPropertyHandling.htm`*
