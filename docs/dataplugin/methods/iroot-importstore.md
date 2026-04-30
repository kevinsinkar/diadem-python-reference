---
title: "IRoot.ImportStore"
description: "Imports a data file with a specified load method. You can only import data stores that are based on the TDM model. Note that you must not define any groups or p"
---

# IRoot.ImportStore

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: ImportStore for Root <DataPlugin>

Imports a data file with a specified load method. You can only import data stores that are based on the TDM model. Note that you must not define any groups or properties for the Root object before calling this method. After importing the data file, you can use the Root object as usual.

## Signature

```python
obj.ImportStore(FileName, Plugin)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadStore(FileName):
    TempFolder = AutoRemove.CreateFolder()

    FileList = Unzip(FileName, TempFolder)

    Root.ImportStore(TempFolder + FileList(0), "ATFX")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_ImportStore_IRoot.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
