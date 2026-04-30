---
title: "ITemplateProperty"
description: "The Property object provides a custom properties template of the data set ( Root ), of a Channel group , or of a Channel in the script interface for internal da"
---

# ITemplateProperty

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: TemplateProperty

The Property object provides a custom properties template of the data set ( Root ), of a Channel group , or of a Channel in the script interface for internal data. The TemplateProperty object is an element of the TemplateProperties collection.

## Python example

```python
oMyPropTemplate = dd.Data.Settings.CustomPropertyTemplate
oMyPropTemplate.RootProperties("MyRootProp").Value = 0
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itemplateproperty-datatype/">DataType</a> | <a href="../../properties/itemplateproperty-name/">Name</a> | <a href="../../properties/itemplateproperty-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/templateproperties/">TemplateProperties</a>.<a href="../../methods/itemplateproperties-add/">Add</a> | <a href="../../collections/templateproperties/">TemplateProperties</a>.<a href="../../methods/itemplateproperties-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_ITemplateProperty.htm`*
