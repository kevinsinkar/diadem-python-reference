---
title: "ITextStream.SkipLine"
description: "Skips a line when reading a TextStream file."
---

# ITextStream.SkipLine

!!! abstract "Method &middot; `Scripting.chm`"
    Method: SkipLine for TextStream

Skips a line when reading a TextStream file.

## Signature

```python
obj.SkipLine
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def SkipOneLine(sFile):
    ForReading = 1; ForWriting = 2
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile= fso.OpenTextFile(sFile, ForWriting, True)
    oMyFile.Write "First Line" + "\r\n" + "Second Line"
    oMyFile = fso.OpenTextFile(sFile, ForReading)
    oMyFile.SkipLine
    SkipOneLine = oMyFile.ReadLine
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_SkipLine_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
