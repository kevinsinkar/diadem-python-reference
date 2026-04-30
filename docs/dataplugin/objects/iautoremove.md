---
title: "IAutoRemove"
description: "The AutoRemove object offers support when working with ZIP archives. The methods allow you to unzip ZIP archives to a temporary folder and automatically delete "
---

# IAutoRemove

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: AutoRemove

The AutoRemove object offers support when working with ZIP archives. The methods allow you to unzip ZIP archives to a temporary folder and automatically delete the files in this folder. Note that a ZIP archive contains exactly one measurement data file. The DataFinder indexes a ZIP file only once, like any other measurement data file. Addressing within the ZIP archive is not possible.

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

## Members

<div markdown="1">
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iautoremove-addexisting/">AddExisting</a> | <a href="../../methods/iautoremove-createfolder/">CreateFolder</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idataplugin/">DataPlugin</a>.<a href="../../properties/idataplugin-autoremove/">AutoRemove</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IAutoRemove.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
