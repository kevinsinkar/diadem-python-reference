---
title: "IDriveCollection.Item"
description: "Returns a single Drive object. You can use this to access a single drive."
---

# IDriveCollection.Item

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Item for Drives

Returns a single Drive object. You can use this to access a single drive.

## Signature

```python
return_value = obj.Item(Key)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
fso = CreateObject("Scripting.FileSystemObject")
oMyDrives = fso.Drives
dd.MsgBox(oMyDrives.Item("C").TotalSize)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Item_IDriveCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
