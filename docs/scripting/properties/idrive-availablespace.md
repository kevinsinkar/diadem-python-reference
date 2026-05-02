---
title: "IDrive.AvailableSpace"
description: "Specifies the size of the available memory of a drive."
---

# IDrive.AvailableSpace

!!! abstract "Property &middot; `Scripting.chm`"
    Property: AvailableSpace for Drive

Specifies the size of the available memory of a drive.

## Signature

```python
obj.AvailableSpace
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveAvailablelSpaceList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + "\t"
        if oMyDrive.IsReady:
            sOutput = sOutput + FormatNumber(oMyDrive.AvailableSpace,0)
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + "\r\n"
    CreateDriveAvailablelSpaceList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_AvailableSpace_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
