---
title: "IDiademProperty"
description: "The Property object provides a property for the Root object, for the ChannelGroup object, or for the Channel object in the script interface for internal data. T"
---

# IDiademProperty

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: Property <Data>

The Property object provides a property for the Root object, for the ChannelGroup object, or for the Channel object in the script interface for internal data. This property is either a DIAdem base property or a custom property. The Property object is an element of the Properties or PropertyList collection.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Properties in DIAdem - Overview</a> for information about properties of files, groups, and channels.</td></tr></table>
</div>

## Python example

```python
for oMyChn in dd.Data.Root.ChannelGroups(1).Channels:
    for oMyProp in oMyChn.Properties:
        if oMyProp.Name == "MyOffset" :
            oMyProp.Value = oMyProp.Value * 2
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademproperty-custom/">Custom</a> | <a href="../../properties/idiademproperty-datatype/">DataType</a> | <a href="../../properties/idiademproperty-displayname/">DisplayName</a> | <a href="../../properties/idiademproperty-element/">Element</a> | <a href="../../properties/idiademproperty-hidden/">Hidden</a> | <a href="../../properties/idiademproperty-name/">Name</a> | <a href="../../properties/idiademproperty-readonly/">ReadOnly</a> | <a href="../../properties/idiademproperty-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/properties/">Properties &lt;Data&gt;</a>.<a href="../../methods/idiademproperties-add/">Add</a> | <a href="../../collections/properties/">Properties &lt;Data&gt;</a>.<a href="../../methods/idiademproperties-item/">Item</a> | <a href="../../collections/propertylist/">PropertyList &lt;Data&gt;</a>.<a href="../../methods/idiadempropertylist-add/">Add</a> | <a href="../../collections/propertylist/">PropertyList &lt;Data&gt;</a>.<a href="../../methods/idiadempropertylist-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademProperty.HTM`*
