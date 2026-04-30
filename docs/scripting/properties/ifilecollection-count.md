---
title: "IFileCollection.Count"
description: "Returns the number of files in a folder."
---

# IFileCollection.Count

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Count for Files

Returns the number of files in a folder.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CountFiles(sFolderSpec):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolderSpec)
    oMyFiles = oMyFolder.Files
    CountFiles = "Number of Files: " + oMyFiles.Count
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Count_IFileCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
