---
title: "IFileInfo"
description: "The Info object contains information about the file that the DataPlugin is currently processing."
---

# IFileInfo

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Info

The Info object contains information about the file that the DataPlugin is currently processing.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("File name", File.Info.FileName)
```

```python
Root.Properties.Add("File name", FromStore.FileInfo.FileName)
```

```python
Root.Properties.Add("File name", Workbook.FileInfo.FileName)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifileinfo-directory/">Directory</a> | <a href="../../properties/ifileinfo-drive/">Drive</a> | <a href="../../properties/ifileinfo-extension/">Extension</a> | <a href="../../properties/ifileinfo-filename/">FileName</a> | <a href="../../properties/ifileinfo-fullpath/">FullPath</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../imeasurementfileio/">File</a>.<a href="../../properties/imeasurementfileio-info/">Info</a> | <a href="../iusisimplifiedstore/">Store</a>.<a href="../../properties/iusisimplifiedstore-fileinfo/">FileInfo</a> | <a href="../iexcelfileio/">Workbook</a>.<a href="../../properties/iexcelfileio-fileinfo/">FileInfo</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Store Object Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IFileInfo.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
