---
title: "IFolder.Name"
description: "Specifies the name of a folder."
---

# IFolder.Name

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Name for Folder

Specifies the name of a folder.

## Signature

```python
obj.Name
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFolderInfo(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    sOutput = "Folder: " + oMyFolder.Name + VBCrLf
    sOutput = sOutput + "Created: " + oMyFolder.DateCreated + VBCrLf
    sOutput = sOutput + "Last Accessed: " + oMyFolder.DateLastAccessed + VBCrLf
    sOutput = sOutput + "Last Modified: " + oMyFolder.DateLastModified
    ShowFolderInfo = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Name_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
