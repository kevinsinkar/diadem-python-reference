---
title: "IDocumentProperties.Remove"
description: "Deletes a custom property of a document. Custom properties are user-defined meta properties from the top level of a document. You can read, create, edit, and de"
---

# IDocumentProperties.Remove

!!! abstract "Method &middot; `FileTagging.chm`"
    Method: Remove for DocumentProperties <Data>

Deletes a custom property of a document. Custom properties are user-defined meta properties from the top level of a document. You can read, create, edit, and delete custom properties. You can only read the other meta properties of a document and edit their values. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf",False, dd.eDocumentTypeAuto)
oMyProperties = oMyDocument.Properties
for oMyProperty in oMyProperties:
    sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value  + "\r\n"
sOut = sOut + "\r\n" + "==After removing custom property==" + "\r\n"
if oMyProperties.Exists("copyright") :
    oMyDocument.Properties.Remove("copyright")
for oMyProperty in oMyProperties:
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

*Source: `FileTagging/methods/DiaCmpnt_method_Remove_IDocumentProperties.htm`*
