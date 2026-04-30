---
title: "FileDateSet"
description: "Sets time and date of files."
---

# FileDateSet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FileDateSet

Sets time and date of files.

## Signature

```python
dd.FileDateSet(FSSourceName, FSDateType, FSDateTime)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The Windows Explorer displays the date of the last file change.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you use two digits to specify the year, DIAdem automatically adds the first two digits of the year.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you use two digits to specify the year, DIAdem automatically adds the first two digits of the year.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The Windows Explorer displays the date of the last file change.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FSSourceName</td>
<td>Specifies the source file or source folder for DIAdem file and folder commands.<div id="exp_FSSourceName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum <a href="../../../varoff/variables/applicationmaxpathlength/">ApplicationMaxPathLength</a> characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
</div></td></tr>
<tr><td width="150">FSDateType</td>
<td>Specifies whether you change the time of file creation, of the last change, or of the last access.<div id="exp_FSDateType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"fdCreate"</pre></donottranslate></td>
<td>Created</td></tr>
<tr><td width="150"><donottranslate><pre>"fdAccess"</pre></donottranslate></td>
<td>Last access</td></tr>
<tr><td width="150"><donottranslate><pre>"fdModify"</pre></donottranslate></td>
<td>Changed</td></tr>
</table>
</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The Windows Explorer displays the date of the last file change.</td></tr></table>
</div></td></tr>
<tr><td width="150">FSDateTime</td>
<td>Specifies date and time in the time format of the operating system.<div id="exp_FSDateTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you use two digits to specify the year, DIAdem automatically adds the first two digits of the year.</td></tr></table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.FileDateSet("C:\\Source.*","fdModify",Date + " " + Time)
```

---

*Source: `ComOff/FileDateSet.htm`*
