---
title: "IDiademDocument.Save"
description: "Saves the document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a doc"
---

# IDiademDocument.Save

!!! abstract "Method &middot; `FileTagging.chm`"
    Method: Save for Document <Data>

Saves the document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.Save()
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
if not(oMyDocument.ReadOnly) :
    oMyDocument.Properties.Add("Modified","Yes",dd.DataTypeString)
    oMyDocument.Save()
sOut = "File path: " + oMyDocument.FilePath + "\r\n"
for oMyProperty in oMyDocument.Properties:
    sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value  + "\r\n"
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `FileTagging/methods/DiaCmpnt_method_Save_IDiademDocument.htm`*
