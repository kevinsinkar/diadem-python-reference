---
title: "DataFileSelDlg"
description: "Opens the dialog box for selective loading, in DIAdem NAVIGATOR."
---

# DataFileSelDlg

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileSelDlg

Opens the dialog box for selective loading, in DIAdem NAVIGATOR.

## Signature

```python
dd.DataFileSelDlg(DataFilename, FileImportFilter)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileImportFilter</span> variable for a file type, enable the <a href="#" data-unresolved="1">Recording mode</a> and open a file with the appropriate filename extension in the <a href="#" data-unresolved="1">Open</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../datafileload/">DataFileLoad</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Visit the <a href="#">DataPlugin website</a> to find existing DataPlugins you can download.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DataFilename</td>
<td>Specifies the name of a data file with the filename extension and the path.<div id="exp_DataFilename">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
</div></td></tr>
<tr><td width="150">FileImportFilter</td>
<td>Specifies which DataPlugin DIAdem uses for loading a data file into the Data Portal.<div id="exp_FileImportFilter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">If you do not specify a DataPlugin, DIAdem automatically uses the DataPlugin assigned to the file type.</p>
<p class="Body">The valid values for this variable vary according to the registered DataPlugin. The following values are valid:</p>
<table class="Borderless"><tr>
<td width="150"><strong>Value of the Variables</strong></td><td width="150"><strong>Meaning</strong></td>
<td><strong>Filename Extension</strong></td></tr><tr>
<td width="150"><span class="Monospace">TDM</span></td><td width="150">DIAdem TDM files</td>
<td><span class="Monospace">TDM</span></td></tr><tr>
<td width="150"><span class="Monospace">TDMS</span></td><td width="150">DIAdem TDM streaming files</td>
<td><span class="Monospace">TDMS</span></td></tr>
<tr><td width="150"><span class="Monospace">LVM</span></td><td width="150">LabVIEW LVM files</td>
<td><span class="Monospace">LVM</span></td></tr>
<tr><td width="150"><span class="Monospace">CSV</span></td><td width="150">Comma-separated values</td>
<td><span class="Monospace">CSV</span></td></tr>
<tr><td width="150"><span class="Monospace">DAT</span></td><td width="150">DIAdem DAT files</td>
<td><span class="Monospace">DAT</span></td></tr>
</table><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileImportFilter</span> variable for a file type, enable the <a href="#" data-unresolved="1">Recording mode</a> and open a file with the appropriate filename extension in the <a href="#" data-unresolved="1">Open</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../datafileload/">DataFileLoad</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Visit the <a href="#">DataPlugin website</a> to find existing DataPlugins you can download.</td></tr></table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.DataFileSelDlg("C:\\Example.tdm","TDM")
```

---

*Source: `ComOff/DataFileSelDlg.htm`*
