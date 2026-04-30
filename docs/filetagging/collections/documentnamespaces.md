---
title: "DocumentNamespaces"
description: "Collection of name spaces in a document. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or a PDF,"
---

# DocumentNamespaces

!!! abstract "Collection &middot; `FileTagging.chm`"
    Collection: DocumentNamespaces <Data>

Collection of name spaces in a document. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
for oMyNameSpaces in oMyDocument.Namespaces:
    sOut = sOut + "Namespace: " + oMyNameSpaces.Name + ", Number of properties:  " + oMyNameSpaces.Properties.Count + "\r\n"
    for oMyProperty in oMyNameSpaces.Properties:
        sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value + "\r\n"
print(sOut)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idocumentnamespaces-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idocumentnamespaces-exists/">Exists</a> | <a href="../../methods/idocumentnamespaces-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idiademdocument/">Document &lt;Data&gt;</a>.<a href="../../properties/idiademdocument-namespaces/">Namespaces</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/Objects/DiaCmpnt_Objects_IDocumentNamespaces.htm`*
