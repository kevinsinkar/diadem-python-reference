---
title: "IFolder.SubFolders"
description: "Returns the folders collection for a Folder object. You can use this to access the subfolders in a folder."
---

# IFolder.SubFolders

!!! abstract "Property &middot; `Scripting.chm`"
    Property: SubFolders for Folder

Returns the folders collection for a Folder object. You can use this to access the subfolders in a folder.

## Signature

```python
return_value = obj.SubFolders
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CountFolders(sFolderSpec):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolderSpec)
    oMySubFolders = oMyFolder.SubFolders
    CountFolders = "Number of folders: " + oMySubFolders.Count
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_SubFolders_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
