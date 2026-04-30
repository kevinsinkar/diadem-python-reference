---
title: "IVbsFileService.UploadResultFileToWorkspace"
description: "Uploads a file to the SystemLink file service in the specified workspace. You can also find the uploaded files in the results of current and completed Analysis "
---

# IVbsFileService.UploadResultFileToWorkspace

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: UploadResultFileToWorkspace for FileService <SystemLink>

Uploads a file to the SystemLink file service in the specified workspace. You can also find the uploaded files in the results of current and completed Analysis Automation tasks. You can then download these files to your computer from the results or open them in SystemLink File Viewer. You can use the UploadResultFileToWorkspace method to define additional properties for the SystemLink file service that enable you to filter the files by procedure, task, or subtask, for example. The properties are not saved in the file, but are assigned to the file in the SystemLink file service. Whether you can execute this method in a task with the specified workspace depends on the privileges of the service or user who executes the task. The UploadResultFileToWorkspace method replaces the UploadResultFile method.

## Signature

```python
sUploadResultFileToWorkspace = Object.UploadResultFileToWorkspace(path, properties, dataplugin, disableDefaultProperties, workspace)
```

## Python example

```python
import win32com
def On_Finalize(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    dd.Report.ActiveSheet.ExportToPDF(ResultsPath + "Result.pdf",False)
    sProperty = AddKeyValue(["Resultpath"],[ResultsPath])
    oContext.FileService.UploadResultFileToWorkspace(ResultsPath + "\\Result.pdf", sProperty, "" ,False, "0aadbc36-9498-4928-94cf-b600eab14562")

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

*Source: `TDMcontext/methods/TDMContext_method_UploadResultFileToWorkspace_IVbsFileService.htm`*
