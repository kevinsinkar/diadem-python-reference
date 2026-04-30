---
title: "IFolder.DateCreated"
description: "Specifies the folder creation date and time."
---

# IFolder.DateCreated

!!! abstract "Property &middot; `Scripting.chm`"
    Property: DateCreated for Folder

Specifies the folder creation date and time.

## Signature

```python
return_value = obj.DateCreated
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

*Source: `Scripting/properties/Scripting_property_DateCreated_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
