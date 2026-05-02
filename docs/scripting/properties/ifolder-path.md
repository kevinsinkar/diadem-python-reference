---
title: "IFolder.Path"
description: "Specifies the path of a folder."
---

# IFolder.Path

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Path for Folder

Specifies the path of a folder.

## Signature

```python
obj.Path
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FolderPath(sFolder):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    FolderPath = "Path: " + oMyFolder.Path
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Path_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
