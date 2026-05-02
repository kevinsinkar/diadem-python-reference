---
title: "IDrive.DriveType"
description: "Returns the drive type."
---

# IDrive.DriveType

!!! abstract "Property &middot; `Scripting.chm`"
    Property: DriveType for Drive

Returns the drive type.

## Signature

```python
obj.DriveType
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveTypeList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + "\t"
        # select oMyDrive.DriveType
        # case 0
        sOutput = sOutput + "Unknown"
        # case 1
        sOutput = sOutput + "Removable"
        # case 2
        sOutput = sOutput + "Fixed"
        # case 3
        sOutput = sOutput + "Network"
        # case 4
        sOutput = sOutput + "CD-ROM"
        # case 5
        sOutput = sOutput + "RAM Disk"
    sOutput = sOutput + "\r\n"
CreateDriveTypeList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_DriveType_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
