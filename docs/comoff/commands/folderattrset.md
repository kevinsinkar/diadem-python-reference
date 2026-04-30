---
title: "FolderAttrSet"
description: "Sets folder attributes."
---

# FolderAttrSet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FolderAttrSet

Sets folder attributes.

## Signature

```python
dd.FolderAttrSet(FSSourceName, FSAttrType)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
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
<tr><td width="150">FSAttrType</td>
<td>Specifies the file attribute or the folder attribute.<div id="exp_FSAttrType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"faNormal"</pre></donottranslate></td>
<td>No bit</td></tr>
<tr><td width="150"><donottranslate><pre>"faReadOnly"</pre></donottranslate></td>
<td>Read only bit</td></tr>
<tr><td width="150"><donottranslate><pre>"faHidden"</pre></donottranslate></td>
<td>Hide bit</td></tr>
<tr><td width="150"><donottranslate><pre>"faArchive"</pre></donottranslate></td>
<td>Archive bit</td></tr>
<tr><td width="150"><donottranslate><pre>"faSystem"</pre></donottranslate></td>
<td>System bit</td></tr>
<tr><td width="150"><donottranslate><pre>"faAnyFile"</pre></donottranslate></td>
<td>All bits</td></tr>
<tr><td width="150"><donottranslate><pre>"faOffline"</pre></donottranslate></td>
<td>Offline bit</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.FolderAttrSet(dd.ScriptReadPath + "L*", "faReadOnly")
```

---

*Source: `ComOff/FolderAttrSet.htm`*
