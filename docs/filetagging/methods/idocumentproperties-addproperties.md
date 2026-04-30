---
title: "IDocumentProperties.AddProperties"
description: "Adds a copy of the property from the top level of a document. The names of the new meta properties correspond to the names of the copied properties plus a prefi"
---

# IDocumentProperties.AddProperties

!!! abstract "Method &middot; `FileTagging.chm`"
    Method: AddProperties for DocumentProperties <Data>

Adds a copy of the property from the top level of a document. The names of the new meta properties correspond to the names of the copied properties plus a prefix. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.AddProperties(Properties, Prefix)
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
for oMyProperty in oMyDocument.Properties:
    sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value  + "\r\n"
oMyDocument.Properties.AddProperties(dd.Data.Root.ChannelGroups(1).Channels(1).Properties,"Example~")
sOut = sOut + "==After adding properties==" + "\r\n"
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

*Source: `FileTagging/methods/DiaCmpnt_method_AddProperties_IDocumentProperties.htm`*
