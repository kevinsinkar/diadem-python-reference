---
title: "IRepDisplayDimensionsInt.Ratio"
description: "Specifies the global ratio of the page height to the page width for worksheets in DIAdem REPORT. DIAdem only includes the Ratio property if you assign the value"
---

# IRepDisplayDimensionsInt.Ratio

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Ratio for DisplayDimensions

Specifies the global ratio of the page height to the page width for worksheets in DIAdem REPORT. DIAdem only includes the Ratio property if you assign the value FALSE to the UseScaledOutput property.

## Signature

```python
obj.Ratio
```

## Python example

```python
oMyDimensions = dd.Report.Settings.Page.Dimensions
oMyDimensions.UseScaledOutput = False
oMyDimensions.Ratio = 1.5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Ratio_IRepDisplayDimensionsInt.htm`*
