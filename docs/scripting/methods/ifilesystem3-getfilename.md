---
title: "IFileSystem3.GetFileName"
description: "Returns the part of the path that corresponds with the name of a file or a folder."
---

# IFileSystem3.GetFileName

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetFileName for FileSystemObject

Returns the part of the path that corresponds with the name of a file or a folder.

## Signature

```python
sGetFileName = Object.GetFileName(Path)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetName(sDrive):
    fso = CreateObject("Scripting.FileSystemObject")
    GetName = fso.GetFileName(sDrive)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetFileName_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
