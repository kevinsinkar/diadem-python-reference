---
title: "IDocumentNamespaces.Exists"
description: "Specifies whether a namespace of a document already exists. Use namespaces to group XML elements in a document."
---

# IDocumentNamespaces.Exists

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Exists for DocumentNamespaces <DataPlugin>

Specifies whether a namespace of a document already exists. Use namespaces to group XML elements in a document.

## Signature

```python
bExists = Object.Exists(sName)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
sNamespace = "http://ns.adobe.com/xap/1.0/"
if Document.Namespaces.Exists(sNamespace):
    oMyNamespaceProps = Document.Namespaces(sNamespace).Properties
    for oMyProp in oMyNamespaceProps:
        Root.Properties.Add(oMyProp.Name, oMyProp.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Exists_IDocumentNamespaces.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
