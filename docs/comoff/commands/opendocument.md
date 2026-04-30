---
title: "OpenDocument"
description: "Returns an object which provides methods and properties for reading or editing the metadata of a document."
---

# OpenDocument

!!! abstract "Command &middot; `ComOff.chm`"
    Command: OpenDocument

Returns an object which provides methods and properties for reading or editing the metadata of a document.

## Signature

```python
return_value = dd.OpenDocument( DocumentFileName , [ ReadOnly ], [ DocumentFileType ])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Do not use the OpenDocument command in TDM Server scripts, because other processes, such as the DataFinder, will not be able to access the opened files. Instead, set the meta properties in the document with the <a href="../../../reportapi/properties/irepsettingsexportint-properties/">Properties for Export</a> property, before you export the layout in XML format, as PDF-, JPEG-, PNG- or TIFF file.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DocumentFileName</td>
<td>Specifies the filename of the document.<div id="exp_DocumentFileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ReadOnly]</td>
<td>Specifies whether DIAdem opens a document in read-only mode or with read and write rights. By default DIAdem opens a document with write and read rights.<div id="exp_ReadOnly">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[DocumentFileType]</td>
<td>Specifies the file types of the document.<div id="exp_DocumentFileType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr>
<td>0 &lt;= DocumentFileType &lt;= 4<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless">
<tr><td><table class="Borderless"><tr><td width="30"><span class="Monospace">0</span></td><td width="120"><span class="Monospace">eDocumentTypeAuto</span></td>
<td>The file type is specified automatically from the filename extension</td></tr>
<tr><td width="30"><span class="Monospace">1</span></td><td width="120"><span class="Monospace">eDocumentTypeXMP</span></td><td>XMPfile (for example *.pdf; *.jpg; *.jpeg; *.png; *.tif; *.tiff)</td></tr>
<tr><td width="30"><span class="Monospace">2</span></td><td width="120"><span class="Monospace">eDocumentTypeWord</span></td><td>XML based Word file (for example *.docx; *.docm; *.dotx; *.dotm)</td></tr>
<tr><td width="30"><span class="Monospace">3</span></td><td width="120"><span class="Monospace">eDocumentTypeExcel</span></td><td>XML based Excel file (for example *.xlsx; *.xltm; *.xltx; *.xltm)</td></tr>
<tr><td width="30"><span class="Monospace">4</span></td><td width="120"><span class="Monospace">eDocumentTypePowerPoint</span></td><td>XML based PowerPoint file (for example *.pptx; *.pptm; *.potx; *.potm)</td></tr>
</table></td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td><a href="../../../filetagging/objects/idiademdocument/">Document &lt;Data&gt; object</a> type return value.</td></tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDocumentTypeAuto` | 0 | The file type is specified automatically from the filename extension |
| `eDocumentTypeXMP` | 1 | XMPfile (for example *.pdf; *.jpg; *.jpeg; *.png; *.tif; *.tiff) |
| `eDocumentTypeWord` | 2 | XML based Word file (for example *.docx; *.docm; *.dotx; *.dotm) |
| `eDocumentTypeExcel` | 3 | XML based Excel file (for example *.xlsx; *.xltm; *.xltx; *.xltm) |
| `eDocumentTypePowerPoint` | 4 | XML based PowerPoint file (for example *.pptx; *.pptm; *.potx; *.potm) |

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
if oMyDocument is None :
    print("Could not open the file.")
else:
    for oMyProperty in oMyDocument.Properties:
        sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value  + "\r\n"
    print(sOut)
```

---

*Source: `ComOff/OpenDocument.htm`*
