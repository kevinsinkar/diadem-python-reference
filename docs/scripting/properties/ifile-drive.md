---
title: "IFile.Drive"
description: "Returns the Drive object for a file. You can use this to access the associated drive."
---

# IFile.Drive

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Drive for File

Returns the Drive object for a file. You can use this to access the associated drive.

## Signature

```python
return_value = obj.Drive
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FileDrive(sFile):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    FileDrive = "Path: " + oMyFile.Drive
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Drive_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
