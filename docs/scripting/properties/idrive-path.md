---
title: "IDrive.Path"
description: "Specifies the path of a drive."
---

# IDrive.Path

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Path for Drive

Specifies the path of a drive.

## Signature

```python
obj.Path
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def RootPath(sDrv):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyDrive = fso.GetDrive(sDrv)
    RootPath = "Root: " + oMyDrive.Path
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Path_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
