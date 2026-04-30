---
title: "IDocumentNamespaces.Count"
description: "Returns the number of namespaces of a document. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or"
---

# IDocumentNamespaces.Count

!!! abstract "Property &middot; `FileTagging.chm`"
    Property: Count for DocumentNamespaces <Data>

Returns the number of namespaces of a document. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.Count
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
sOut =  "Number of namesspaces:  " + oMyDocument.Namespaces.Count + "\r\n"
for oMyNameSpaces in oMyDocument.Namespaces:
    sOut = sOut + "Namespace: " + oMyNameSpaces.Name + "\r\n"
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/properties/DiaCmpnt_property_Count_IDocumentNamespaces.htm`*
