---
title: "IDrive.VolumeName"
description: "Specifies the drive name."
---

# IDrive.VolumeName

!!! abstract "Property &middot; `Scripting.chm`"
    Property: VolumeName for Drive

Specifies the drive name.

## Signature

```python
obj.VolumeName
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

*Source: `Scripting/properties/Scripting_property_VolumeName_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
