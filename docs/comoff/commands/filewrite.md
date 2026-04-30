---
title: "FileWrite"
description: "Writes a line without a concluding line break into an ASCII file."
---

# FileWrite

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FileWrite

Writes a line without a concluding line break into an ASCII file.

## Signature

```python
dd.FileWrite(FileName, RecMode, FileLine)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the target file already exists DIAdem overwrites this file without a confirmation prompt.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the ASCII file is not open when DIAdem executes the <span class="Monospace">FileWrite</span> command, DIAdem opens this file and closes the file again. If the file is already open, DIAdem does not close the file after the command is executed.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="#" data-unresolved="1">TextFileWriteLn</a> function to write in text files. This function also supports long text and Unicode characters.  Use the <a href="#" data-unresolved="1">TextFileReadLn</a> function to read text files.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileName</td>
<td>Specifies the file name.<div id="exp_FileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
</div></td></tr>
<tr><td width="150">RecMode</td>
<td>Specifies whether DIAdem writes the text into a newly created ASCII file or whether DIAdem appends the text to the contents of an existing ASCII file.<div id="exp_RecMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
<td>0 &lt;= RecMode &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">RecMode</span> variable can accept the following values:</p>
<table class="Borderless">
<tr>
<td width="150"><span class="Monospace">0</span></td>
<td>Create new file</td>
</tr>
<tr>
<td width="150"><span class="Monospace">1</span></td>
<td>Append to file</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">FileLine</td>
<td>Specifies the text that DIAdem writes into a text file.<div id="exp_FileLine">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 255 characters</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/FileWrite.htm`*
