---
title: "IDiademUSIElement"
description: "The Element object provides a single element in the script interface for internal data. Depending on whether an element of the internal data is a data set ( Roo"
---

# IDiademUSIElement

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: Element <Data>

The Element object provides a single element in the script interface for internal data. Depending on whether an element of the internal data is a data set ( Root ), a group ( ChannelGroup ), or a channel ( Channel ), the Element object has additional properties. Use the IsKindOf method to determine the type of an element. Refer to Working with the Elements Collection and the Element Object for general information on working with the elements.

## Python example

```python
for oMySelectedElement in dd.Portal.Structure.Selection:
    if oMySelectedElement.IsKindOf(dd.eDataRoot) :
        dd.MsgBoxDisp ("Root: " + oMySelectedElement.Name)
    elif oMySelectedElement.IsKindOf(dd.eDataChannelGroup) :
        dd.MsgBoxDisp ("ChannelGroup: " + oMySelectedElement.Name)
    elif oMySelectedElement.IsKindOf(dd.eDataChannel) :
        dd.MsgBoxDisp ("Channel: " + oMySelectedElement.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademusielement-name/">Name</a> | <a href="../../properties/idiademusielement-properties/">Properties</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademusielement-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../idiademproperty/">Property &lt;Data&gt;</a>.<a href="../../properties/idiademproperty-element/">Element</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademUSIElement.HTM`*
