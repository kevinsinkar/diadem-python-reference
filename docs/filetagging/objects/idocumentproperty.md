---
title: "IDocumentProperty"
description: "The DocumentProperty <Data> object provides the meta properties of the document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF fil"
---

# IDocumentProperty

!!! abstract "Object &middot; `FileTagging.chm`"
    Object: DocumentProperty <Data>

The DocumentProperty <Data> object provides the meta properties of the document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

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
<p><a href="../../properties/idocumentproperty-custom/">Custom</a> | <a href="../../properties/idocumentproperty-datatype/">DataType</a> | <a href="../../properties/idocumentproperty-name/">Name</a> | <a href="../../properties/idocumentproperty-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/documentproperties/">DocumentProperties &lt;Data&gt;</a>.<a href="../../methods/idocumentproperties-add/">Add</a> | <a href="../../collections/documentproperties/">DocumentProperties &lt;Data&gt;</a>.<a href="../../methods/idocumentproperties-item/">Item</a> | <a href="../../collections/documentreadonlyproperties/">DocumentReadOnlyProperties &lt;Data&gt;</a>.<a href="../../methods/idocumentreadonlyproperties-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/Objects/DiaCmpnt_Objects_IDocumentProperty.htm`*
