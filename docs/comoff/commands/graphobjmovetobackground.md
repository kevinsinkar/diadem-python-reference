---
title: "GraphObjMoveToBackground"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMoveToBackground command:"
---

# GraphObjMoveToBackground

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphObjMoveToBackground (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMoveToBackground command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the methods <a href="../../../reportapi/methods/irepctrlzorderint-move/">Move</a>, <a href="../../../reportapi/methods/irepctrlzorderint-movetobackground/">MoveToBackground</a>, and <a href="../../../reportapi/methods/irepctrlzorderint-movetoforeground/">MoveToForeground</a>, to move an object in front of or behind other objects in a worksheet in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.ActiveSheet.Objects(1).Position.ZOrder.MoveToBackground()
```

---

*Source: `ComOff/GraphObjMoveToBackground.htm`*
