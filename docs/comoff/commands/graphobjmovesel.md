---
title: "GraphObjMoveSel"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMoveSel command:"
---

# GraphObjMoveSel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphObjMoveSel (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMoveSel command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the methods <a href="../../../reportapi/methods/irepctrlzorderint-move/">Move</a>, <a href="../../../reportapi/methods/irepctrlzorderint-movetobackground/">MoveToBackground</a>, and <a href="../../../reportapi/methods/irepctrlzorderint-movetoforeground/">MoveToForeground</a>, to move an object in front of or behind other objects in a worksheet in DIAdem REPORT. Use the <a href="../../../reportapi/collections/selectedobjects/">SelectedObjects</a> collection to access all selected elements in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
for oMySelectedObject in dd.Report.SelectedObjects:
    oMySelectedObject.Position.ZOrder.MoveToForeground()
```

---

*Source: `ComOff/GraphObjMoveSel.htm`*
