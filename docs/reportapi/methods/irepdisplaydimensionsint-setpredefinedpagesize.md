---
title: "IRepDisplayDimensionsInt.SetPredefinedPageSize"
description: "Specifies the size and the format of worksheets in DIAdem REPORT."
---

# IRepDisplayDimensionsInt.SetPredefinedPageSize

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetPredefinedPageSize for DisplayDimensions

Specifies the size and the format of worksheets in DIAdem REPORT.

## Signature

```python
obj.SetPredefinedPageSize(PageFormat, PageOrientation)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePageFormatA4` | 0 | DIN A4 format |
| `ePageFormatA3` | 1 | DIN A3 format |
| `ePageFormatA5` | 2 | DIN A5 format |
| `ePageFormatLetter` | 3 | Letter format |
| `ePageFormatExecutive` | 4 | Executive format |
| `ePageFormatLegal` | 5 | Legal format |
| `ePageFormatLedger` | 6 | Ledger format |
| `ePageOrientationLandscape` | 0 | Landscape |
| `ePageOrientationPortrait` | 1 | Portrait |

## Python example

```python
dd.Report.Settings.Page.Dimensions.SetPredefinedPageSize(dd.ePageFormatA3,dd.ePageOrientationLandscape)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetPredefinedPageSize_IRepDisplayDimensionsInt.htm`*
