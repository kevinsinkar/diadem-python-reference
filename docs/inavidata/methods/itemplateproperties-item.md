---
title: "ITemplateProperties.Item"
description: "Returns the TemplateProperty object that is associated with a specific name or a specific index, in the script interface for internal data."
---

# ITemplateProperties.Item

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Item for TemplateProperties

Returns the TemplateProperty object that is associated with a specific name or a specific index, in the script interface for internal data.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because this method is always the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyProp = dd.Data.Settings.CustomPropertyTemplate.RootProperties.Item(1)
dd.MsgBoxDisp ("Property name: " + oMyProp.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Item_ITemplateProperties.htm`*
