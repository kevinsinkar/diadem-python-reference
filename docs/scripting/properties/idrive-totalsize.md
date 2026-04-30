---
title: "IDrive.TotalSize"
description: "Specifies the total memory space of a drive."
---

# IDrive.TotalSize

!!! abstract "Property &middot; `Scripting.chm`"
    Property: TotalSize for Drive

Specifies the total memory space of a drive.

## Signature

```python
obj.TotalSize
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveTotalSizeList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + VBTab
        if oMyDrive.IsReady:
            sOutput = sOutput + FormatNumber(oMyDrive.TotalSize,0)
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + VBCrLf
    CreateDriveTotalSizeList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_TotalSize_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
