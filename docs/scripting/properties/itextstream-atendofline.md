---
title: "ITextStream.AtEndOfLine"
description: "Checks whether the read pointer is just before the end of line of a TextStream file."
---

# ITextStream.AtEndOfLine

!!! abstract "Property &middot; `Scripting.chm`"
    Property: AtEndOfLine for TextStream

Checks whether the read pointer is just before the end of line of a TextStream file.

## Signature

```python
obj.AtEndOfLine
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadEndOfLine(sFile):
    ForReading = 1
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.OpenTextFile(sFile, ForReading, False)
    while oMyFile.AtEndOfLine != True:
        sOutput = oMyFile.Read(1)
    oMyFile.Close
    ReadEndOfLine = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_AtEndOfLine_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
