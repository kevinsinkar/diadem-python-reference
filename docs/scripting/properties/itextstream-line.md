---
title: "ITextStream.Line"
description: "Specifies the current line number of the file pointer in a TextStream file. After the file is open, the property has the value 1."
---

# ITextStream.Line

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Line for TextStream

Specifies the current line number of the file pointer in a TextStream file. After the file is open, the property has the value 1.

## Signature

```python
obj.Line
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetFileLines(sFile):
    Const ForReading = 1
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFile = fso.OpenTextFile(sFile, ForReading, False)
    sOutput = oMyFile.ReadAll
    GetFileLines = oMyFile.Line
    oMyFile.Close
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Line_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
