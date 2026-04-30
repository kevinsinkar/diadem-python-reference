---
title: "GraphObjPositionGet"
description: "The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjPositionGet command:"
---

# GraphObjPositionGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GraphObjPositionGet (Obsolete)

The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjPositionGet command:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete. Use the object-oriented interface in DIAdem REPORT instead. Use the methods <a href="../../../reportapi/methods/irepd2axisxint-convertpagexpositiontoxaxisvalue/">ConvertPageXPositionToXAxisValue</a> and <a href="../../../reportapi/methods/irepd2axisxint-convertxaxisvaluetopagexposition/">ConvertXAxisValueToPageXPosition</a> to convert a page coordinate into an axis coordinate in a 2D axis system in DIAdem REPORT.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
</div>

## Python example

```python
dd.Report.ActiveSheet.Objects(1).XAxis.ConvertPageXPositionToXAxisValue()
dd.Report.ActiveSheet.Objects(1).YAxis.ConvertPageYPositionToYAxisValue()
```

---

*Source: `ComOff/GraphObjPositionGet.htm`*
