---
title: "IRepSheetDimensionsInt.Orientation"
description: "Specifies the page orientation of the current worksheet in DIAdem REPORT. DIAdem only includes the property Orientation if you assign the value TRUE to the UseL"
---

# IRepSheetDimensionsInt.Orientation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Orientation for SheetDimensions

Specifies the page orientation of the current worksheet in DIAdem REPORT. DIAdem only includes the property Orientation if you assign the value TRUE to the UseLocalSettings property.

## Signature

```python
obj.Orientation
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePageOrientationLandscape` | 0 | Landscape |
| `ePageOrientationPortrait` | 1 | Portrait |

## Python example

```python
dd.MsgBoxDisp(dd.Report.ActiveSheet.Dimensions.Orientation)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Orientation_IRepSheetDimensionsInt.htm`*
