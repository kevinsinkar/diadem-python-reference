---
title: "IVbsContextASDeinit.FileService"
description: "Returns the FileService <SystemLink> object. The FileService <SystemLink> object allows you to upload files to the SystemLink file service. You can also find th"
---

# IVbsContextASDeinit.FileService

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: FileService for ContextFinalize <Analysis Automation>

Returns the FileService <SystemLink> object. The FileService <SystemLink> object allows you to upload files to the SystemLink file service. You can also find the uploaded files in the results of current and completed analysis automation tasks. You can download them from there or open them in the SystemLink File Viewer.

## Signature

```python
return_value = obj.FileService
```

## Python example

```python
def On_Finalize(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    dd.Report.ActiveSheet.ExportToPDF(ResultsPath + "Result.pdf",False)
    sProperty = "{\"Resultpath\": \"" + ResultsPath.replace("\\", "\\\\") + "\"}"
    oContext.FileService.UploadResultFile(ResultsPath + "\\Result.pdf", sProperty, "" ,False)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_FileService_IVbsContextASDeinit.htm`*
