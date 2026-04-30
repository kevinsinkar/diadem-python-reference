---
title: "IDiademProperty.Hidden"
description: "Specifies in the script interface for internal data, whether DIAdem displays the property of a data element in the user interface. In DIAdem you can hide only t"
---

# IDiademProperty.Hidden

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Hidden for Property <Data>

Specifies in the script interface for internal data, whether DIAdem displays the property of a data element in the user interface. In DIAdem you can hide only the register properties. However, the properties are maintained in the associated collections.

## Signature

```python
obj.Hidden
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>DIAdem hides the register properties by default.</td></tr></table>
</div>

## Python example

```python
dd.MsgBoxDisp (dd.Data.Root.ActiveChannelGroup.Channels(1).Properties("RegisterInt1").Hidden)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Hidden_IDiademProperty.HTM`*
