---
title: "FileExportFilter"
description: "Specifies the storage method you use to save data from the DIAdem Data Portal to a file. If you do not specify a storage method, DIAdem saves the data with the "
---

# FileExportFilter

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: FileExportFilter

Specifies the storage method you use to save data from the DIAdem Data Portal to a file. If you do not specify a storage method, DIAdem saves the data with the TDM DataPlugin.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To specify the value of the <span class="Monospace">FileExportFilter</span> variable for DataPlugins, enable the<a href="#" data-unresolved="1"> Recording mode</a> and select a file type in the <a href="#" data-unresolved="1">Save As</a> dialog box. In the script recorded in the script editor, you then receive the value of the variable as a parameter of the <a href="../../../comoff/commands/datafilesave/">DataFileSave</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not save data in the TDM format, group information or properties, for example, may be left out because some formats cannot save all information.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you save data in the CSV format, DIAdem saves only the first channel group. To save other channel groups, you must save the channel groups selectively.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you save data in the CSV format, DIAdem uses a tabulator as the separator.</td></tr></table>
</div>

---

*Source: `VarOff/FileExportFilter.htm`*
