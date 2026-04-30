---
title: "TemplateProperties"
description: "Collection of all the properties of a custom properties template for the Root object, the ChannelGroup object, or the Channel object in the script interface for"
---

# TemplateProperties

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: TemplateProperties

Collection of all the properties of a custom properties template for the Root object, the ChannelGroup object, or the Channel object in the script interface for internal data. You can use the TemplateProperties collection to access custom properties templates and to add and delete custom properties templates.

## Python example

```python
oMyPropTemplate = dd.Data.Settings.CustomPropertyTemplate
oMyPropTemplate.RootProperties.Add("MyRootProp", 2)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itemplateproperties-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itemplateproperties-add/">Add</a> | <a href="../../methods/itemplateproperties-exists/">Exists</a> | <a href="../../methods/itemplateproperties-item/">Item</a> | <a href="../../methods/itemplateproperties-remove/">Remove</a> | <a href="../../methods/itemplateproperties-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idatatemplate/">CustomPropertyTemplate</a>.<a href="../../properties/idatatemplate-channelgroupproperties/">ChannelGroupProperties</a> | <a href="../../objects/idatatemplate/">CustomPropertyTemplate</a>.<a href="../../properties/idatatemplate-channelproperties/">ChannelProperties</a> | <a href="../../objects/idatatemplate/">CustomPropertyTemplate</a>.<a href="../../properties/idatatemplate-rootproperties/">RootProperties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_ITemplateProperties.htm`*
