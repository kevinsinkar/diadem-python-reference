---
title: "IDocumentNamespaces.Exists"
description: "Specifies whether a namespace of a document already exists. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in X"
---

# IDocumentNamespaces.Exists

!!! abstract "Method &middot; `FileTagging.chm`"
    Method: Exists for DocumentNamespaces <Data>

Specifies whether a namespace of a document already exists. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
sNameSpace = "http://ns.adobe.com/xap/1.0/mm/"
if oMyDocument.Namespaces.Exists(sNameSpace) :
    sOut = sOut + "Namespace exists: " + oMyDocument.Namespaces(sNameSpace).Name
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/methods/DiaCmpnt_method_Exists_IDocumentNamespaces.htm`*
