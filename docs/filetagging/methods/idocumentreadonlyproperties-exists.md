---
title: "IDocumentReadOnlyProperties.Exists"
description: "Checks whether a meta property already exists in a specific namespace of a document. The meta properties in a specific namespace are read-only. Use namespaces t"
---

# IDocumentReadOnlyProperties.Exists

!!! abstract "Method &middot; `FileTagging.chm`"
    Method: Exists for DocumentReadOnlyProperties <Data>

Checks whether a meta property already exists in a specific namespace of a document. The meta properties in a specific namespace are read-only. Use namespaces to identify XML elements clearly in a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
for oMyNameSpaces in oMyDocument.Namespaces:
    if oMyNameSpaces.Properties.Exists("Copyright") :
        oMyProperty = oMyNameSpaces.Properties("Copyright")
        sOut = sOut + "Namespace: " + oMyNameSpaces.Name + "\r\n"
        sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value + "\r\n"
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/methods/DiaCmpnt_method_Exists_IDocumentReadOnlyProperties.htm`*
