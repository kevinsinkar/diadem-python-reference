---
title: "FolderUnzip"
description: "Unzips a ZIP archive to a folder."
---

# FolderUnzip

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FolderUnzip

Unzips a ZIP archive to a folder.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FolderZipName</td>
<td>Specifies the name of the ZIP archive.<div id="exp_FolderZipName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">FolderZipPath</td>
<td>Specifies the name of the folder.<div id="exp_FolderZipPath">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Returns the value <span class="Monospace">0</span> if the function has executed successfully. Returns the value <span class="Monospace">-2147024809</span> if the ZIP archive <span class="Monospace">FolderZipName</span> does not exist. Returns <span class="Monospace">-2147090424</span> if the <span class="Monospace">FolderZipPath</span> folder does not exist. Returns the value <span class="Monospace">-2147467259</span> if another error occurred. The return value is a <a href="#" data-unresolved="1">Integer</a> type.</td></tr>
</table>
</div>

## Python example

```python
dd.FolderUnZip("C:\\Myfolder1\\pack.zip", "C:\\Myfolder2")
```

---

*Source: `ComOff/FolderUnzip.htm`*
