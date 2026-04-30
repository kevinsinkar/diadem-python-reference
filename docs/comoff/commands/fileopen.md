---
title: "FileOpen"
description: "Opens ASCII files for reading or writing."
---

# FileOpen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FileOpen

Opens ASCII files for reading or writing.

## Signature

```python
dd.FileOpen(FileName, FileMode)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for or creates ASCII files in the SCRIPT user folder.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <a href="../textfileopen/">TextFileOpen</a> function to open text files. Use the <a href="#" data-unresolved="1">TextFileClose</a> function to close text files. These functions also support long text and Unicode characters.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileName</td>
<td>Specifies the filename.<div id="exp_FileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum <a href="../../../varoff/variables/applicationmaxpathlength/">ApplicationMaxPathLength</a> characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
</div></td></tr>
<tr><td width="150">FileMode</td>
<td>Specifies whether you write into a new ASCII file, extend the contents of an existing ASCII file, or read from an existing file.<div id="exp_FileMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
<td>0 &lt;= FileMode &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">FileMode</span> variable can accept three values:</p>
<table class="Borderless">
<tr>
<td width="150"><span class="Monospace">0</span></td>
<td>Create new file and open file for writing.</td>
</tr>
<tr>
<td width="150"><span class="Monospace">1</span></td>
<td>Append to existing file and open file for writing.</td>
</tr>
<tr>
<td width="150"><span class="Monospace">2</span></td>
<td>Open for reading.</td>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.FileOpen(dd.DataReadPath + "Text.asc",0)
```

---

*Source: `ComOff/FileOpen.htm`*
