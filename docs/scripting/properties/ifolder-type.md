---
title: "IFolder.Type"
description: "Specifies the type of a folder."
---

# IFolder.Type

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Type for Folder

Specifies the type of a folder.

## Signature

```python
obj.Type
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFolderType(sFolder):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    ShowFolderType = oMyFolder.Type
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Type_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
