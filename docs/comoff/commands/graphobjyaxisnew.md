---
title: "GraphObjYAxisNew"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjYAxisNew command:"
---

# GraphObjYAxisNew

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphObjYAxisNew (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjYAxisNew command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the <a href="../../../reportapi/methods/irepd2axisylistint-add/">Add</a> method to add a y-axis to a 2D axis system in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.ActiveSheet.Objects(1).YAxisList.Add()
```

---

*Source: `ComOff/GraphObjYAxisNew.htm`*
