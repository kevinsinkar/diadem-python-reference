---
title: "ITextStream.AtEndOfStream"
description: "Checks whether the read pointer is just before the end of the file of a TextStream file."
---

# ITextStream.AtEndOfStream

!!! abstract "Property &middot; `Scripting.chm`"
    Property: AtEndOfStream for TextStream

Checks whether the read pointer is just before the end of the file of a TextStream file.

## Signature

```python
obj.AtEndOfStream
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadFile(sFile):
    ForReading = 1
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.OpenTextFile(sFile, ForReading, False)
    while oMyFile.AtEndOfStream != True:
        sOutput = sOutput + oMyFile.ReadLine + "\r\n"
    oMyFile.Close
    ReadFile = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_AtEndOfStream_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
