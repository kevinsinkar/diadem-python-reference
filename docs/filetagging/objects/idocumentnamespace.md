---
title: "IDocumentNamespace"
description: "The DocumentNamespace <Data> object provides the namespace in a document. Use namespaces to identify XML elements clearly in a document. A document may be an Of"
---

# IDocumentNamespace

!!! abstract "Object &middot; `FileTagging.chm`"
    Object: DocumentNamespace <Data>

The DocumentNamespace <Data> object provides the namespace in a document. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

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
<p><a href="../../properties/idocumentnamespace-name/">Name</a> | <a href="../../properties/idocumentnamespace-properties/">Properties</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/documentnamespaces/">DocumentNamespaces &lt;Data&gt;</a>.<a href="../../methods/idocumentnamespaces-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/Objects/DiaCmpnt_Objects_IDocumentNamespace.htm`*
