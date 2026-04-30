---
title: "IAutoRemove.CreateFolder"
description: "Creates a new, unique folder reserved for the automatic deletion process. The automatic deletion of the folder and its files occurs as soon as the DataPlugin no"
---

# IAutoRemove.CreateFolder

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: CreateFolder for AutoRemove

Creates a new, unique folder reserved for the automatic deletion process. The automatic deletion of the folder and its files occurs as soon as the DataPlugin no longer requires these files.

## Signature

```python
sCreateFolder = Object.CreateFolder([sBaseFolder])
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

*Source: `DataPlugin/Methods/DataPlugin_method_CreateFolder_IAutoRemove.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
