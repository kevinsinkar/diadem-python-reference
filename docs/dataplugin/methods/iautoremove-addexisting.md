---
title: "IAutoRemove.AddExisting"
description: "Reserves a file or a folder for deletion. The folder is deleted automatically, as soon as the DataPlugin has stopped importing the data."
---

# IAutoRemove.AddExisting

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddExisting for AutoRemove

Reserves a file or a folder for deletion. The folder is deleted automatically, as soon as the DataPlugin has stopped importing the data.

## Signature

```python
obj.AddExisting(sFileOrFolder)
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

    # further instructions

    AutoRemove.AddExisting("C:\Temp\")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddExisting_IAutoRemove.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
