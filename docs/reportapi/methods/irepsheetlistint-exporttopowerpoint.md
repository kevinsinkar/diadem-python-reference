---
title: "IRepSheetListInt.ExportToPowerPoint"
description: "Exports all worksheets from DIAdem REPORT to a PowerPoint file. If the PowerPoint file already exists, DIAdem overwrites the PowerPoint file. DIAdem generates a"
---

# IRepSheetListInt.ExportToPowerPoint

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ExportToPowerPoint for Sheets

Exports all worksheets from DIAdem REPORT to a PowerPoint file. If the PowerPoint file already exists, DIAdem overwrites the PowerPoint file. DIAdem generates a PPTX file with the same number of slides as there are pages in your report. Every page displays the name and layout of the page as a graphic. You can customize the PowerPoint export template to match your corporate layout. To do so, edit or replace the PPTX file PowerPointTemplate.pptx . The file is in the Resource folder of your DIAdem program folder. This template must contain at least two wildcards in the user-defined layout: one for text and one for graphics. You can position both placeholders anywhere in the slide master. The PPT export does not require that PowerPoint is installed. To edit the template, you require PowerPoint as of version 2007.

## Signature

```python
obj.ExportToPowerPoint(FileName)
```

## Python example

```python
dd.Report.Sheets.ExportToPowerPoint("d:\\MySheets")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ExportToPowerPoint_IRepSheetListInt.htm`*
