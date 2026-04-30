---
title: "IDiademProperty.Name"
description: "Returns the name of a property in the script interface for internal data. In the Data Preparation Procedure DIAdem uses the term Identifier for the name of a pr"
---

# IDiademProperty.Name

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Name for Property <Data>

Returns the name of a property in the script interface for internal data. In the Data Preparation Procedure DIAdem uses the term Identifier for the name of a property.

## Signature

```python
obj.Name
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Properties in DIAdem - Overview</a> for information about properties of files, groups, and channels.</td></tr></table>
</div>

## Python example

```python
dd.MsgBoxDisp (dd.Data.Root.Properties(2).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Name_IDiademProperty.HTM`*
