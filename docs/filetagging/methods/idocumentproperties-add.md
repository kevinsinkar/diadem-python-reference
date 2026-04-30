---
title: "IDocumentProperties.Add"
description: "Adds a custom property of a document. Custom properties are user-defined meta properties from the top level of a document. You can read, create, edit, and delet"
---

# IDocumentProperties.Add

!!! abstract "Method &middot; `FileTagging.chm`"
    Method: Add for DocumentProperties <Data>

Adds a custom property of a document. Custom properties are user-defined meta properties from the top level of a document. You can read, create, edit, and delete custom properties. You can only read the other meta properties of a document and edit their values. After saving the document with the Save method, you can search for new custom properties. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
return_value = obj.Add(Name, Value, [DataType])
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
if not(oMyDocument.ReadOnly) :
    oMyDocument.Properties.Add("Modified","Yes", dd.DataTypeDocumentString)
    oMyDocument.Save()
sOut = "File path: " + oMyDocument.FilePath + "\r\n"
for oMyProperty in oMyDocument.Properties:
    sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value  + "\r\n"
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/methods/DiaCmpnt_method_Add_IDocumentProperties.htm`*
