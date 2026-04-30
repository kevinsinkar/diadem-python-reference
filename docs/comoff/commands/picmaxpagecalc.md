---
title: "PicMaxPageCalc"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicMaxPageCalc command:"
---

# PicMaxPageCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: PicMaxPageCalc (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicMaxPageCalc command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use <a href="../../../reportapi/methods/irepsubsheetsint-recalculate/">Recalculate</a> to recalculate the number of table pages of an automatically extending 2D table in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.Sheets(1).SubSheets.Recalculate()
```

---

*Source: `ComOff/PicMaxPageCalc.htm`*
