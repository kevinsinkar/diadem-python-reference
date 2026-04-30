---
title: "IRepReportInt.AppendedFullPath"
description: "Specifies the complete name of a layout loaded to the existing layout in DIAdem REPORT."
---

# IRepReportInt.AppendedFullPath

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AppendedFullPath for Report

Specifies the complete name of a layout loaded to the existing layout in DIAdem REPORT.

## Signature

```python
obj.AppendedFullPath
```

## Python example

```python
dd.Report.AppendLayout("Demo.tdr")
print("Fullpath: " + dd.Report.AppendedFullPath + "\r\n" + "Layout file name: " + dd.Report.AppendedFileName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AppendedFullPath_IRepReportInt.htm`*
