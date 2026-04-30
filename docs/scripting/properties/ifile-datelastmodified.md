---
title: "IFile.DateLastModified"
description: "Specifies the last file modification date and time."
---

# IFile.DateLastModified

!!! abstract "Property &middot; `Scripting.chm`"
    Property: DateLastModified for File

Specifies the last file modification date and time.

## Signature

```python
return_value = obj.DateLastModified
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFileInfo(sFile):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    sOutput = "File: " + oMyFile.Name + VBCrLf
    sOutput = sOutput + "Created: " + oMyFile.DateCreated + VBCrLf
    sOutput = sOutput + "Last Accessed: " + oMyFile.DateLastAccessed + VBCrLf
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

*Source: `Scripting/properties/Scripting_property_DateLastModified_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
