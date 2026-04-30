---
title: "PicPrint"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicPrint command:"
---

# PicPrint

!!! abstract "Command &middot; `ComOff.chm`"
    Command: PicPrint (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicPrint command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the methods <a href="../../../reportapi/methods/irepsheetlistint-printall/">PrintAll</a> and <a href="../../../reportapi/methods/irepsheetlistint-printrange/">PrintRange</a> to print DIAdem REPORT worksheets:<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.Sheets.PrintAll()
dd.Report.Sheets.PrintRange(2,4)
```

---

*Source: `ComOff/PicPrint.htm`*
