---
title: "IRepSelectedObjectsListInt.Exists"
description: "Checks whether an object with a specific name already exists in the objects selected in the current worksheet of DIAdem REPORT."
---

# IRepSelectedObjectsListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for SelectedObjects

Checks whether an object with a specific name already exists in the objects selected in the current worksheet of DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.Report.SelectedObjects.Exists("2DTable1"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepSelectedObjectsListInt.htm`*
