---
title: "IDrive.FreeSpace"
description: "Specifies the size of the free memory of a drive."
---

# IDrive.FreeSpace

!!! abstract "Property &middot; `Scripting.chm`"
    Property: FreeSpace for Drive

Specifies the size of the free memory of a drive.

## Signature

```python
obj.FreeSpace
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveSpaceList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + VBTab
        if oMyDrive.IsReady:
            sOutput = sOutput + FormatNumber(oMyDrive.FreeSpace,0)
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + VBCrLf
    CreateDriveSpaceList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_FreeSpace_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
