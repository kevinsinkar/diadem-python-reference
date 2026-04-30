---
title: "FileChnOffs"
description: "Specifies the channel offset, that is the number of values between two channel values, when DAT files are imported via header."
---

# FileChnOffs

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: FileChnOffs

Specifies the channel offset, that is the number of values between two channel values, when DAT files are imported via header.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Do not enter a channel offset when you import binary block files that do not contain a header that can be skipped and if you want to read in all the values of the files. For binary block files that contain a header that can be skipped, the channel offset specifies the number of records between two values in a channel. For ASCII files with a CRLF separator, the channel offset specifies the number of values between 2 successive values that belong to one channel.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem uses this variable to selectively load and save DAT files. The command <a href="../../../comoff/commands/dataloadhdfile/">DataLoadHdFile</a> loads the respective data set properties of DAT files and assigns the respective value to the variable.</td></tr></table>
</div>

---

*Source: `VarOff/FileChnOffs.htm`*
