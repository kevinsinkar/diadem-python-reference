---
title: "IFolder.Size"
description: "Specifies the size of a folder including subfolders."
---

# IFolder.Size

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Size for Folder

Specifies the size of a folder including subfolders.

## Signature

```python
obj.Size
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFolderSize(sFolder):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    ShowFolderSize = "Size: " + oMyFolder.Size
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Size_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
