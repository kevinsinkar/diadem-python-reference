---
title: "IFile.DateLastAccessed"
description: "Specifies the last file access date and time."
---

# IFile.DateLastAccessed

!!! abstract "Property &middot; `Scripting.chm`"
    Property: DateLastAccessed for File

Specifies the last file access date and time.

## Signature

```python
return_value = obj.DateLastAccessed
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFileInfo(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    sOutput = "File: " + oMyFile.Name + "\r\n"
    sOutput = sOutput + "Created: " + oMyFile.DateCreated + "\r\n"
    sOutput = sOutput + "Last Accessed: " + oMyFile.DateLastAccessed + "\r\n"
    sOutput = sOutput + "Last Modified: " + oMyFile.DateLastModified
    ShowFileInfo = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_DateLastAccessed_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
