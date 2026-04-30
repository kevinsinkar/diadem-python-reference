---
title: "IFileSystem3.DriveExists"
description: "Checks whether a drive exists."
---

# IFileSystem3.DriveExists

!!! abstract "Method &middot; `Scripting.chm`"
    Method: DriveExists for FileSystemObject

Checks whether a drive exists.

## Signature

```python
bDriveExists = Object.DriveExists(DriveSpec)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def DriveStatus(sDrv):
    fso = CreateObject("Scripting.FileSystemObject")
    if fso.DriveExists(sDrv):
        sOutput = ("Drive " + sDrv + " exists.")
    else:
        sOutput = ("Drive " + sDrv + " doesn't exist.")
    DriveStatus = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_DriveExists_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
