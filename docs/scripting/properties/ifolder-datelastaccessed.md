---
title: "IFolder.DateLastAccessed"
description: "Specifies the last folder access date and time."
---

# IFolder.DateLastAccessed

!!! abstract "Property &middot; `Scripting.chm`"
    Property: DateLastAccessed for Folder

Specifies the last folder access date and time.

## Signature

```python
return_value = obj.DateLastAccessed
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFolderInfo(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    sOutput = "Folder: " + oMyFolder.Name + "\r\n"
    sOutput = sOutput + "Created: " + oMyFolder.DateCreated + "\r\n"
    sOutput = sOutput + "Last Accessed: " + oMyFolder.DateLastAccessed + "\r\n"
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

*Source: `Scripting/properties/Scripting_property_DateLastAccessed_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
