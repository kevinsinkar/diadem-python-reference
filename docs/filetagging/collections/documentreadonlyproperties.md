---
title: "DocumentReadOnlyProperties"
description: "Collection of all meta properties in a specific namespace of a document. The meta properties in a specific namespace are read-only. Use namespaces to identify X"
---

# DocumentReadOnlyProperties

!!! abstract "Collection &middot; `FileTagging.chm`"
    Collection: DocumentReadOnlyProperties <Data>

Collection of all meta properties in a specific namespace of a document. The meta properties in a specific namespace are read-only. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

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
<p><a href="../../properties/idocumentreadonlyproperties-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idocumentreadonlyproperties-exists/">Exists</a> | <a href="../../methods/idocumentreadonlyproperties-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idocumentnamespace/">DocumentNamespace &lt;Data&gt;</a>.<a href="../../properties/idocumentnamespace-properties/">Properties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/Objects/DiaCmpnt_Objects_IDocumentReadOnlyProperties.htm`*
