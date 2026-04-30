---
title: "FileDlgFileName"
description: "Receives a list of all the files, including the paths, that you select in the dialog box for loading or for saving."
---

# FileDlgFileName

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: FileDlgFileName

Receives a list of all the files, including the paths, that you select in the dialog box for loading or for saving.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you use the <a href="../../../comoff/commands/filenameget/">FileNameGet</a> command to open a file selection dialog box and select several files, the <span class="Monospace">FileDlgFileName</span> variable receives the filenames separated by a vertical line, for example:<br attr="ext"/><span class="Monospace">FileDlgFileName = "C:\My Files\First.tdm|C:\My Files\Second.tdm|C:\My Files\Third.tdm"</span></td></tr></table>
</div>

---

*Source: `VarOff/FileDlgFileName.htm`*
