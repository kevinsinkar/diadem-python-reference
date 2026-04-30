---
title: "GraphObjSelect"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjSelect command:"
---

# GraphObjSelect

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphObjSelect (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjSelect command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the <a href="../../../reportapi/methods/irepbasectrlint-select/">Select</a> method to select an object in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.ActiveSheet.Objects(1).Select()
```

---

*Source: `ComOff/GraphObjSelect.htm`*
