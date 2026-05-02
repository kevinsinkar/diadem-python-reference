---
title: "IFile.DateCreated"
description: "Specifies the file creation date and time."
---

# IFile.DateCreated

!!! abstract "Property &middot; `Scripting.chm`"
    Property: DateCreated for File

Specifies the file creation date and time.

## Signature

```python
return_value = obj.DateCreated
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

*Source: `Scripting/properties/Scripting_property_DateCreated_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
