---
title: "DocumentProperties"
description: "Collection of changeable meta properties that are not assigned to a namespace, from the top level of a document. A document may be an Office file in XML format "
---

# DocumentProperties

!!! abstract "Collection &middot; `FileTagging.chm`"
    Collection: DocumentProperties <Data>

Collection of changeable meta properties that are not assigned to a namespace, from the top level of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document. The five properties name , description , title , author , and datetime are the base properties of a document. They are permanent and cannot be deleted.

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
for oMyProperty in oMyDocument.Properties:
    sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value  + "\r\n"
print(sOut)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idocumentproperties-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idocumentproperties-add/">Add</a> | <a href="../../methods/idocumentproperties-addproperties/">AddProperties</a> | <a href="../../methods/idocumentproperties-exists/">Exists</a> | <a href="../../methods/idocumentproperties-item/">Item</a> | <a href="../../methods/idocumentproperties-remove/">Remove</a> | <a href="../../methods/idocumentproperties-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idiademdocument/">Document &lt;Data&gt;</a>.<a href="../../properties/idiademdocument-properties/">Properties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/Objects/DiaCmpnt_Objects_IDocumentProperties.htm`*
