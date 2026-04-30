---
title: "CreateExcelWorkbook"
description: "Creates a new Excel workbook or opens an existing Excel file. Excel does not need to be installed on your computer."
---

# CreateExcelWorkbook

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CreateExcelWorkbook

Creates a new Excel workbook or opens an existing Excel file. Excel does not need to be installed on your computer.

## Signature

```python
return_value = dd.CreateExcelWorkbook([ExcelFileName])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[ExcelFileName]</td>
<td>Specifies the Excel file that DIAdem opens. If you do not specify an Excel file, the command creates an Excel workbook with an empty worksheet named <span class="Monospace">Sheet1</span>.<div id="exp_ExcelFileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Workbook object</a> type. The Workbook object corresponds to an Excel workbook.</td></tr>
</table>
</div>

## Python example

```python
oMyWorkbook = dd.CreateExcelWorkbook()
oMySheet = oMyWorkbook.Worksheets(1)
for iRow in range( 1, 1000+1):
    for jCol in range( 1, 20+1):
        oMyCell = oMySheet.Cells(iRow, jCol)
        oMyCell.Value = Round(dd.Random(100))
        if oMyCell.Value == 47 : oMyCell.Interior.Color = dd.RGB(255, 0, 0)
    oMyWorkbook.SaveAs(dd.DataWritePath + "Test.xlsx")
```

---

*Source: `ComOff/CreateExcelWorkbook.htm`*
