---
title: "IFolderCollection.Item"
description: "Returns a single Folder object. You can use this to access a single folder."
---

# IFolderCollection.Item

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Item for Folders

Returns a single Folder object. You can use this to access a single folder.

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
oMySubFolders = oMyFolder.SubFolders
dd.MsgBox(oMySubFolders.Item("Resource").Size)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Item_IFolderCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
