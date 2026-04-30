---
title: "GraphObjScalingUpdate"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjScalingUpdate command:"
---

# GraphObjScalingUpdate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphObjScalingUpdate (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjScalingUpdate command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the methods <a href="../../../reportapi/methods/irepd2axisint-updatescaling/">UpdateScaling for 2DAxisSystem</a>, <a href="../../../reportapi/methods/irepd3axisint-updatescaling/">UpdateScaling for 3DAxisSystem</a>, and <a href="../../../reportapi/methods/ireppolarint-updatescaling/">UpdateScaling for PolarSystem</a> to refresh the values DIAdem REPORT uses when an axis system is automatically scaled.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.ActiveSheet.Objects(1).UpdateScaling()
```

---

*Source: `ComOff/GraphObjScalingUpdate.htm`*
