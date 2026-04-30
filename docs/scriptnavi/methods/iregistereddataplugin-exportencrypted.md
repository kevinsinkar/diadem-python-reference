---
title: "IRegisteredDataPlugin.ExportEncrypted"
description: "Exports an encrypted DataPlugin registered on your computer into a URI file."
---

# IRegisteredDataPlugin.ExportEncrypted

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: ExportEncrypted for RegisteredDataPlugin <Navigator>

Exports an encrypted DataPlugin registered on your computer into a URI file.

## Signature

```python
bExportEncrypted = Object.ExportEncrypted(Name)
```

## Python example

```python
oMyDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
oMyDataPlugin = oMyDataPlugins("LGR")
bExport = oMyDataPlugin.ExportEncrypted("D:\\LGRCrypt_New.uri")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_ExportEncrypted_IRegisteredDataPlugin.htm`*
