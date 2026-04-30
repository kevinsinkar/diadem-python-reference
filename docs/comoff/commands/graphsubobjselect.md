---
title: "GraphSubObjSelect"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSubObjSelect command:"
---

# GraphSubObjSelect

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphSubObjSelect (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSubObjSelect command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the methods <a href="../../../reportapi/methods/irepd2selectedsubobjectslistint-add2d/">Add2D for 2DSelectedElements </a>, <a href="../../../reportapi/methods/ireptable2dselectedsubobjectslistint-add2dtable/">Add2DTable for 2DTableSelectedElements</a>, <a href="../../../reportapi/methods/irepd3selectedsubobjectslistint-add3d/">Add3D for 3DSelectedElements</a>, <a href="../../../reportapi/methods/ireptable3dselectedsubobjectslistint-add3dtable/">Add3DTable for 3DTableSelectedElements</a>, <a href="../../../reportapi/methods/irepcommentselectedsubobjectslistint-addcomment/">AddComment for CommentSelectedElements</a>, and <a href="../../../reportapi/methods/ireppolarselectedsubobjectslistint-addpolar/">AddPolar for PolarSelectedElements</a> to select an object in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.SelectedObjects(1).SelectedElements.Add(dd.e2DElementCurve,1)
```

---

*Source: `ComOff/GraphSubObjSelect.htm`*
