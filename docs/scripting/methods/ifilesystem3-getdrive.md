---
title: "IFileSystem3.GetDrive"
description: "Returns a drive object that is associated with a path."
---

# IFileSystem3.GetDrive

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetDrive for FileSystemObject

Returns a drive object that is associated with a path.

## Signature

```python
return_value = obj.GetDrive(DriveSpec)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetDriveObject(sPath):
    fso = CreateObject("Scripting.FileSystemObject")
    GetDriveObject = fso.GetDrive(fso.GetDriveName(sPath))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetDrive_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
