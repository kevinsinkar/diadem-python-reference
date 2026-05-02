---
title: "IDrive.FileSystem"
description: "Returns the file system of a drive."
---

# IDrive.FileSystem

!!! abstract "Property &middot; `Scripting.chm`"
    Property: FileSystem for Drive

Returns the file system of a drive.

## Signature

```python
obj.FileSystem
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveFileSystemList():
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + "\t"
        if oMyDrive.IsReady:
            sOutput = sOutput + oMyDrive.FileSystem
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + "\r\n"
    CreateDriveFileSystemList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_FileSystem_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
