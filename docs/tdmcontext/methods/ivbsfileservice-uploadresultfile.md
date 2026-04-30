---
title: "IVbsFileService.UploadResultFile"
description: "Uploads a file to the SystemLink file service for the workspace of the associated task. You can also find the uploaded files in the results of current and compl"
---

# IVbsFileService.UploadResultFile

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: UploadResultFile for FileService <SystemLink>

Uploads a file to the SystemLink file service for the workspace of the associated task. You can also find the uploaded files in the results of current and completed Analysis Automation tasks. You can then download these files to your computer from the results or open them in SystemLink File Viewer. You can use the UploadResultFile method to define additional properties for the SystemLink file service that enable you to filter the files by procedure, task, or subtask, for example. The properties are not saved in the file, but are assigned to the file in the SystemLink file service. Whether you can upload a file in the task's workspace depends on the privileges of the service or user who executes the task. Instead of the UploadResultFile method, use the UploadResultFileToWorkspace method to specify the workspace as well.

## Signature

```python
sUploadResultFile = Object.UploadResultFile(path, properties, dataplugin, disableDefaultProperties)
```

## Python example

```python
import win32com
def On_Finalize(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    dd.Report.ActiveSheet.ExportToPDF(ResultsPath + "Result.pdf",False)
    sProperty = AddKeyValue(["Resultpath"],[ResultsPath])
    oContext.FileService.UploadResultFile(ResultsPath + "\\Result.pdf", sProperty, "" ,False)

def AddKeyValue(sKeyArray,sValueArray):
    oJsonParser = dd.CreateJsonParser()
    oMyObject = win32com.client.Dispatch("Scripting.Dictionary")
    for iCount in range( 0, len(sKeyArray)-1):
        oMyObject.Add(sKeyArray(iCount), sValueArray(iCount))
    AddKeyValue = oJsonParser.Serialize(oMyObject, False)
    return AddKeyValue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_UploadResultFile_IVbsFileService.htm`*
