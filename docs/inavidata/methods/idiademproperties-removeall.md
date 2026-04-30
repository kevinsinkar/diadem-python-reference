---
title: "IDiademProperties.RemoveAll"
description: "Deletes all custom properties from the Properties collection in the script interface for internal data."
---

# IDiademProperties.RemoveAll

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: RemoveAll for Properties <Data>

Deletes all custom properties from the Properties collection in the script interface for internal data.

## Signature

```python
obj.RemoveAll()
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The <a href="../../collections/properties/">Properties</a> collection contains the base properties and the custom properties. You cannot delete base properties.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.ChannelGroups(1).Properties.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_RemoveAll_IDiademProperties.HTM`*
