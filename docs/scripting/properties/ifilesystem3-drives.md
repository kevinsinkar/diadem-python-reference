---
title: "IFileSystem3.Drives"
description: "Returns the Drives collection of the FileSystemObject object. You can use this to access drives."
---

# IFileSystem3.Drives

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Drives for FileSystemObject

Returns the Drives collection of the FileSystemObject object. You can use this to access drives.

## Signature

```python
return_value = obj.Drives
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + VBTab
        if oMyDrive.DriveType = 3:
            sOutput = sOutput + oMyDrive.ShareName
            ElseIf oMyDrive.IsReady :
            sOutput = sOutput + oMyDrive.VolumeName
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + VBCrLf
    CreateDriveList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Drives_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
