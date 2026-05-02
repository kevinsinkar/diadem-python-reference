---
title: "ITextStream.Column"
description: "Specifies the current column number of the file pointer in a text stream file. After the file is open, the property has the value 1."
---

# ITextStream.Column

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Column for TextStream

Specifies the current column number of the file pointer in a text stream file. After the file is open, the property has the value 1.

## Signature

```python
obj.Column
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetFileColumn(sFile):
    ForReading = 1
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.OpenTextFile(sFile, ForReading, False)
    while oMyFile.AtEndOfLine != True:
        sOutput = oMyFile.Read(1)
    GetFileColumn = oMyFile.Column
    oMyFile.Close
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Column_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
