---
title: "DirListGet"
description: "Generates a list with filenames."
---

# DirListGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DirListGet

Generates a list with filenames.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Sorting with the <span class="Monospace">DirSortType</span> variable is case sensitive. Usually sorts in ascending order. For example, if DIAdem finds the filenames <span class="Monospace">FILE.txt</span> and <span class="Monospace">company.txt</span>, the program enters the filename in uppercase before the filename in lowercase. If you sort by date/time, DIAdem first finds the newest files.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DirSearchPath</td>
<td>Specifies on which drive and in which folder DIAdem searches for the files.<div id="exp_DirSearchPath">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">DirSearchName</td>
<td>Specifies the name of the file that DIAdem searches for in the specified path.<div id="exp_DirSearchName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">DirSortType</td>
<td>Specifies how DIAdem sorts the list it finds.<div id="exp_DirSortType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"filename"</pre></donottranslate></td>
<td>Filename</td></tr>
<tr><td width="150"><donottranslate><pre>"extension"</pre></donottranslate></td>
<td>Filename extension</td></tr>
<tr><td width="150"><donottranslate><pre>"filesize"</pre></donottranslate></td>
<td>File size</td></tr>
<tr><td width="150"><donottranslate><pre>"Date/Time"</pre></donottranslate></td>
<td>Date/Time</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[FileLstFilter]</td>
<td>Specifies the information that DIAdem saves. The default value of the <span class="Monospace">FileLstFilter</span> variable is <span class="Monospace">onlyFilenames</span>.<div id="exp_FileLstFilter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"onlyFilenames"</pre></donottranslate></td>
<td>Only filenames</td></tr>
<tr><td width="150"><donottranslate><pre>"onlyDirectorynames"</pre></donottranslate></td>
<td>Only path names</td></tr>
<tr><td width="150"><donottranslate><pre>"Filenames"</pre></donottranslate></td>
<td>Filenames and filename extensions</td></tr>
<tr><td width="150"><donottranslate><pre>"FullFilenames"</pre></donottranslate></td>
<td>Complete filenames</td></tr>
<tr><td width="150"><donottranslate><pre>"FullFilenamesRecursive"</pre></donottranslate></td>
<td>Recursive after complete filenames</td></tr>
<tr><td width="150"><donottranslate><pre>"DirectorynamesRecursive"</pre></donottranslate></td>
<td>Recursive after path names</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Variant variable</a> type. The return value contains a zero-based array with the entries that the command has found.</td></tr>
</table>
</div>

## Python example

```python
vFoundFiles = dd.DirListGet("C:\\", "*.*", "filename", "FullFilenames")
if isinstance(vFoundFiles, tuple) :
    for iCount in range( 0, len(vFoundFiles)-1):
        strAll = strAll + vFoundFiles(iCount) + "\r\n"
    dd.MsgBoxDisp(strAll)
    hFile=dd.TextFileOpen(dd.ScriptWritePath+ "FileList.asc", dd.eTextFileAttributeCreate or dd.eTextFileAttributeUnicode or dd.eTextFileAttributeWrite or dd.eTextFileAttributeDenyNone)
    dd.TextFileWriteln(hFile, strAll)
    dd.TextFileClose(hFile)
```

---

*Source: `ComOff/DirListGet.htm`*
