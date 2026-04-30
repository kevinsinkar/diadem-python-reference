---
title: "IDataPlugin.Unzip"
description: "Unzips a ZIP archive to a specified folder. The unzipped files are automatically deleted as soon as the DataPlugin no longer requires these files."
---

# IDataPlugin.Unzip

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Unzip for DataPlugin

Unzips a ZIP archive to a specified folder. The unzipped files are automatically deleted as soon as the DataPlugin no longer requires these files.

## Signature

```python
vUnzip = Object.Unzip(ZipArchive, TargetFolder)
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

*Source: `DataPlugin/Methods/DataPlugin_method_Unzip_IDataPlugin.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
