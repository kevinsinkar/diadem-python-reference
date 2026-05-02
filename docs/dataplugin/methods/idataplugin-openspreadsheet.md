---
title: "IDataPlugin.OpenSpreadsheet"
description: "Uses a specified DataPlugin to open an Excel file. To create this DataPlugin use the file reader Only filename in the Configure DataPlugin dialog box. The DataP"
---

# IDataPlugin.OpenSpreadsheet

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: OpenSpreadsheet for DataPlugin

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Uses a specified DataPlugin to open an Excel file. To create this DataPlugin use the file reader Only filename in the Configure DataPlugin dialog box. The DataPlugin cannot access Excel files that are password protected.

## Signature

```python
return_value = obj.OpenSpreadsheet(FileName, [SpreadsheetType])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eXls` | 1 | Excel file created with Excel 2003 or an earlier version. |
| `eXlsx` | 2 | Excel file created with Excel 2007 or Excel 2010. |
| `eOds` | 3 | Excel file created with OpenOffice. |
| `eCsv` | 4 | Excel file created in the CSV format (Character Separated Values). |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadStore(File):
    oExcelFile = OpenSpreadsheet("C:\ExcelExample.xls")
    Root.Properties.Add("Author",oExcelFile.WorkbookInfo.Author)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_OpenSpreadsheet_IDataPlugin.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
