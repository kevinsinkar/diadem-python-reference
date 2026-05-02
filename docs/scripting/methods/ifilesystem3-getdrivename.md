---
title: "IFileSystem3.GetDriveName"
description: "Returns the part of a path that corresponds with the name of the drive."
---

# IFileSystem3.GetDriveName

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetDriveName for FileSystemObject

Returns the part of a path that corresponds with the name of the drive.

## Signature

```python
sGetDriveName = Object.GetDriveName(Path)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetDrive(sDrive):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    GetDrive = fso.GetDriveName(sDrive)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetDriveName_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
