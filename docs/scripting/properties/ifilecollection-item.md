---
title: "IFileCollection.Item"
description: "Returns a single File object. You can use this to access a single file."
---

# IFileCollection.Item

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Item for Files

Returns a single File object. You can use this to access a single file.

## Signature

```python
return_value = obj.Item(Key)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
fso = win32com.client.Dispatch("Scripting.FileSystemObject")
oMyFolder = fso.GetFolder(dd.ProgramDrv)
oMyFiles = oMyFolder.Files
dd.MsgBox(oMyFiles.Item("DIAdem.exe").Size)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Item_IFileCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
