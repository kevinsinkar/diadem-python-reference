---
title: "ReportMasterDel"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterDel command:"
---

# ReportMasterDel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ReportMasterDel (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterDel command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the <a href="../../../reportapi/methods/irepreportmasterlayoutint-disconnect/">Disconnect</a> method to disconnect a layout from a master layout in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.Settings.MasterLayout.Disconnect()
```

---

*Source: `ComOff/ReportMasterDel.htm`*
