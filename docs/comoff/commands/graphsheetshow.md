---
title: "GraphSheetShow"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetShow command:"
---

# GraphSheetShow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphSheetShow (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetShow command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the methods <a href="../../../reportapi/methods/irepsheetint-activate/">Activate</a> and <a href="../../../reportapi/methods/irepreportint-refresh/">Refresh</a> to enable and then update a worksheet in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.Sheets(2).Activate()
dd.Report.Refresh()
```

---

*Source: `ComOff/GraphSheetShow.htm`*
