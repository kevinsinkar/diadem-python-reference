---
title: "IRepPageDefaultSettingsInt.LockUpdate"
description: "Specifies that the display in DIAdem REPORT does not refresh. For example, if you add several worksheets to a script, this property speeds up the execution cons"
---

# IRepPageDefaultSettingsInt.LockUpdate

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LockUpdate for PageDefaultSettings

Specifies that the display in DIAdem REPORT does not refresh. For example, if you add several worksheets to a script, this property speeds up the execution considerably. If you set this property within a script, reset the property before the end of the script. Use the Refresh method to refresh the view.

## Signature

```python
obj.LockUpdate
```

## Python example

```python
dd.Report.Settings.Page.LockUpdate = True
dd.WndShow("REPORT","MAXIMIZE")
sMySheetname = dd.Report.ActiveSheet.Name
for i in range( 1, 10+1):
    dd.Report.Sheets.Copy(sMySheetname, sMySheetname+"_Copy" + i, 2)
dd.Report.Refresh()
dd.Report.Settings.Page.LockUpdate = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LockUpdate_IRepPageDefaultSettingsInt.htm`*
