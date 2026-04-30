---
title: "IDocumentReadProperties.Exists"
description: "Checks whether a property with a specific name already exists in a document. A document can be an Office file in XML format, a PDF, JPEG, PNG, or TIFF file."
---

# IDocumentReadProperties.Exists

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Exists for DocumentProperties <DataPlugin>

Checks whether a property with a specific name already exists in a document. A document can be an Office file in XML format, a PDF, JPEG, PNG, or TIFF file.

## Signature

```python
bExists = Object.Exists(sName)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if Document.Properties.Exists("author"):
    if Document.Properties("author").Value = "Meier":
        sNamespace = "http://ns.adobe.com/xap/1.0/"
        if Document.Namespaces.Exists(sNamespace):
            oMyNamespaceProps = Document.Namespaces(sNamespace).Properties
            for oMyProp in oMyNamespaceProps:
                Root.Properties.Add(oMyProp.Name, oMyProp.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Exists_IDocumentReadProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
