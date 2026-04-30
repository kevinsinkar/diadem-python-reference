---
title: "IDiademDocument"
description: "The Document <Data> object provides the properties and methods for accessing the meta properties of a document. A document may be an Office file in XML format o"
---

# IDiademDocument

!!! abstract "Object &middot; `FileTagging.chm`"
    Object: Document <Data>

The Document <Data> object provides the properties and methods for accessing the meta properties of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

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
<p><a href="../../properties/idiademdocument-filepath/">FilePath</a> | <a href="../../properties/idiademdocument-filetype/">FileType</a> | <a href="../../properties/idiademdocument-namespaces/">Namespaces</a> | <a href="../../properties/idiademdocument-properties/">Properties</a> | <a href="../../properties/idiademdocument-readonly/">ReadOnly</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademdocument-save/">Save</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/Objects/DiaCmpnt_Objects_IDiademDocument.htm`*
