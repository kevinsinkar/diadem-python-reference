---
title: "TextFileEOL"
description: "Specifies the end-of-line character of a text file. The function checks the end-of-line character of the first line. By transferring the end-of-line character t"
---

# TextFileEOL

!!! abstract "Command &middot; `ComOff.chm`"
    Command: TextFileEOL

Specifies the end-of-line character of a text file. The function checks the end-of-line character of the first line. By transferring the end-of-line character to the TextFileOpen function, you can speed up the opening of a text file.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
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
<tr><td width="150">TextFileAttribute</td>
<td>Specifies how DIAdem creates or opens a text file. You can connect various attributes with logic operators.<div id="exp_TextFileAttribute">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>-2147483648 &lt;= TextFileAttribute &lt;= 2147483647</td></tr>
</table>
<table class="Borderless">
<tr>
<td style="width: 30">0</td>
<td width="150"><span class="Monospace">eTextFileAttributeRead</span></td>
<td>Opens a text file in read-only mode.</td>
</tr>
<tr>
<td style="width: 30">1</td>
<td width="150"><span class="Monospace">eTextFileAttributeWrite</span></td>
<td>Opens a text file in read and write mode. When opening a file, DIAdem skips to the end of the file and appends the texts to be written.</td>
</tr>
<tr>
<td style="width: 30">4</td>
<td width="150"><span class="Monospace">eTextFileAttributeANSI</span></td>
<td>Encodes a text file in ANSI.</td>
</tr>
<tr>
<td style="width: 30">8</td>
<td width="150"><span class="Monospace">eTextFileAttributeUnicode</span></td>
<td>Encodes a text file in Unicode.</td>
</tr>
<tr>
<td style="width: 30">16</td>
<td width="150"><span class="Monospace">eTextFileAttributeUTF8</span></td>
<td>Encodes a text file in UTF8. This attribute is only available when the text file is read.</td>
</tr>
<tr>
<td style="width: 30">32</td>
<td width="150"><span class="Monospace">eTextFileAttributeWriteBuffer</span></td>
<td>
<table class="Borderless">
<tr>
<td>Opens a text file in write mode. When writing, DIAdem uses a buffer in order to accelerate the writing. The buffer increases the risk that not all data is saved on the hard disk if the program crashes.</td>
</tr>
</table></td>
</tr>
<tr>
<td style="width: 30">32768</td>
<td width="150"><span class="Monospace">eTextFileAttributeCreate</span></td>
<td>Generates a text file and overwrites any file of the same name in the specified folder without requesting confirmation.</td>
</tr>
<tr>
<td style="width: 30">1048576</td>
<td width="150"><span class="Monospace">eTextFileAttributeExclusive</span></td>
<td>Opens a text file with exclusive read and write rights.</td>
</tr>
<tr>
<td style="width: 30">2097152</td>
<td width="150"><span class="Monospace">eTextFileAttributeDenyWrite</span></td>
<td>Opens a text file as read-only.</td>
</tr>
<tr>
<td style="width: 30">4194304</td>
<td width="150"><span class="Monospace">eTextFileAttributeDenyRead</span></td>
<td>Stops other applications from reading a text file at the same time as DIAdem.</td>
</tr>
<tr>
<td style="width: 30">8388608</td>
<td width="150"><span class="Monospace">eTextFileAttributeDenyNone</span></td>
<td>Allows other applications to access a text file simultaneously with DIAdem.</td>
</tr>
<tr>
<td style="width: 30">16777216</td>
<td width="150"><span class="Monospace">eTextFileAttributenoAutoClose</span></td>
<td>Specifies that DIAdem does not automatically close a text file at the end of a script.</td>
</tr>
<tr>
<td style="width: 30">33554432</td>
<td width="150"><span class="Monospace">eTextFileAttributeLogDIAdemMsg</span></td>
<td>Specifies that DIAdem writes its <a href="#" data-unresolved="1">Logfile</a> into the specified text file.</td>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies the line end character. TextFileLineEnd type return value.<div id="exp_TextFileLineEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Auto"</pre></donottranslate></td>
<td>Automatic</td></tr>
<tr><td width="150"><donottranslate><pre>"CR"</pre></donottranslate></td>
<td>CR (carriage return)</td></tr>
<tr><td width="150"><donottranslate><pre>"LF"</pre></donottranslate></td>
<td>LF (line feed)</td></tr>
<tr><td width="150"><donottranslate><pre>"CRLF"</pre></donottranslate></td>
<td>CRLF (carriage return with line feed)</td></tr>
<tr><td width="150"><donottranslate><pre>"LFCR"</pre></donottranslate></td>
<td>LFCR (line feed with carriage return)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTextFileAttributeRead` | 0 | Opens a text file in read-only mode. |
| `eTextFileAttributeWrite` | 1 | Opens a text file in read and write mode. When opening a file, DIAdem skips to the end of the file and appends the texts to be written. |
| `eTextFileAttributeANSI` | 4 | Encodes a text file in ANSI. |
| `eTextFileAttributeUnicode` | 8 | Encodes a text file in Unicode. |
| `eTextFileAttributeUTF8` | 16 | Encodes a text file in UTF8. This attribute is only available when the text file is read. |
| `eTextFileAttributeCreate` | 32768 | Generates a text file and overwrites any file of the same name in the specified folder without requesting confirmation. |
| `eTextFileAttributeExclusive` | 1048576 | Opens a text file with exclusive read and write rights. |
| `eTextFileAttributeDenyWrite` | 2097152 | Opens a text file as read-only. |
| `eTextFileAttributeDenyRead` | 4194304 | Stops other applications from reading a text file at the same time as DIAdem. |
| `eTextFileAttributeDenyNone` | 8388608 | Allows other applications to access a text file simultaneously with DIAdem. |

## Python example

```python
strFile = dd.ScriptReadPath + "NewText.txt"
strEOL = dd.TextFileEOL(strFile, dd.eTextFileAttributeRead)
intMyHandle = dd.TextFileOpen(strFile, dd.eTextFileAttributeRead, strEOL)
intLineCount = 0
while True:
    strMyText = dd.TextFileReadLn(intMyHandle)
    if (not strMyText == None) :
        intLineCount = intLineCount+1
        dd.MsgBoxDisp(strMyText,"MB_OK")
    if (strMyText == None):
            break
intMyError = dd.TextFileClose(intMyHandle)
```

---

*Source: `ComOff/TextFileEOL.htm`*
