---
title: "IDriveCollection.Count"
description: "Returns the number of drives."
---

# IDriveCollection.Count

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Count for Drives

Returns the number of drives.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CountDrives():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    CountDrives = "Number of drives: " + oMyDrives.Count
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Count_IDriveCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
