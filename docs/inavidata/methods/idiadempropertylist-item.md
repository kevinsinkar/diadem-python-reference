---
title: "IDiademPropertyList.Item"
description: "Returns a single property of the Root object, the ChannelGroup object, or the Channel object which belongs to a specified index."
---

# IDiademPropertyList.Item

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Item for PropertyList <Data>

Returns a single property of the Root object, the ChannelGroup object, or the Channel object which belongs to a specified index.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the Item method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
dd.Report.Events.OnDropPage = "MyOnDropPageEvent"

def MyOnDropPageEvent(Context, DropContext):
    if DropContext.IsKindOf(dd.eDropDIAdemElement) :
        oMyDropElements = DropContext.DiademElements
        sOutput = oMyDropElements.Count + " dropped elements:"
        for i in range( 1, oMyDropElements.Count+1):
            sOutput = sOutput + "\r\n" + "Name: " + oMyDropElements.Item(i).Name
    elif DropContext.IsKindOf(dd.eDropDIAdemProperty) :
        oMyDropProperties = DropContext.DiademProperties
        sOutput = oMyDropProperties.Count + " dropped properties:"
        for i in range( 1, oMyDropProperties.Count+1):
            sOutput = sOutput + "\r\n" + "Name: " + oMyDropProperties.Item(i).Name + "\t" + "DisplayName: " + oMyDropProperties.Item(i).DisplayName
    print(sOutput)
    Context.DoProceed = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Item_IDiademPropertyList.htm`*
