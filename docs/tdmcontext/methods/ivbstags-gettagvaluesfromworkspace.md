---
title: "IVbsTags.GetTagValuesFromWorkspace"
description: "Returns the value of a SystemLink tag in the specified workspace. Whether you can execute this method in a task with the specified workspace depends on the perm"
---

# IVbsTags.GetTagValuesFromWorkspace

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: GetTagValuesFromWorkspace for Tags <SystemLink>

Returns the value of a SystemLink tag in the specified workspace. Whether you can execute this method in a task with the specified workspace depends on the permissions of the service or user who starts the task. Use the GetTagValuesFromWorkspace method instead of the GetTagValues method to also specify the workspace.

## Signature

```python
sGetTagValuesFromWorkspace = Object.GetTagValuesFromWorkspace(path, workspace)
```

## Python example

```python
import win32com
import datetime
def On_Run_AnalysisProcedure(oContext):
    oJsonParser = dd.CreateJsonParser()
    aMyArray = ["Key 1","Key 2"]
    sJsonString = oJsonParser.Serialize(aMyArray)
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    sProperty = AddKeyValue(["Resultpath","Procedure"],[ResultsPath, oContext.TaskExecution.Procedure.Name])
    oContext.Tags.CreateOrUpdateTagToWorkspace("task.id." + oContext.TaskExecution.Id, 1, sJsonString, sProperty, True, "0aadbc36-9498-4928-94cf-b600eab14562")
    sValue = TimeStampedValue("47", "1")
    oContext.Tags.UpdateTagTimestampedValueInWorkspace("task.id." + oContext.TaskExecution.Id, sValue, "0aadbc36-9498-4928-94cf-b600eab14562")
    sReturn = oContext.Tags.GetTagValuesFromWorkspace("task.id." + oContext.TaskExecution.Id, "0aadbc36-9498-4928-94cf-b600eab14562")

def TimeStampedValue(sValue,sType):
    oJsonParser = dd.CreateJsonParser()
    oMySubobject = win32com.client.Dispatch("Scripting.Dictionary")
    oMyMainObject = win32com.client.Dispatch("Scripting.Dictionary")

    oMySubobject.Add("type", sType)
    oMySubobject.Add("value", sValue)

    oMyMainObject.Add("value", oMySubobject)
    oMyMainObject.Add("timestamp", oJsonParser.CreateDateTime(datetime.datetime.now(), False))
    TimeStampedValue = oJsonParser.Serialize(oMyMainObject, False)
    return TimeStampedValue

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

*Source: `TDMcontext/methods/TDMContext_method_GetTagValuesFromWorkspace_IVbsTags.htm`*
