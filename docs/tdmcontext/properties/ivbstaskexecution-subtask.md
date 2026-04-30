---
title: "IVbsTaskExecution.SubTask"
description: "Returns the SubTaskInfo <Analysis Automation> object in Analysis Automation. The SubTaskInfo <Analysis Automation> object provides information on the subtask be"
---

# IVbsTaskExecution.SubTask

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: SubTask for TaskExecution <Analysis Automation>

Returns the SubTaskInfo <Analysis Automation> object in Analysis Automation. The SubTaskInfo <Analysis Automation> object provides information on the subtask being executed.

## Signature

```python
return_value = obj.SubTask
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    sReturn = "ID of current task: " + oContext.TaskExecution.Id + "\r\n"
    sReturn = sReturn + "Subtask ID of current task: " + oContext.TaskExecution.SubTask.Id + "\r\n"
    sReturn = sReturn + "Procedure ID of excecutable task in the Tasks list: " + oContext.TaskExecution.Procedure.Id + "\r\n"
    sReturn = sReturn + "Procedure name of excecutable task in the Tasks list: " + oContext.TaskExecution.Procedure.Name + "\r\n"
    sReturn = sReturn + "Task ID of excecutable task in the Tasks list: " + oContext.TaskExecution.Task.Id  + "\r\n"
    sReturn = sReturn + "Task name of excecutable task in the Tasks list: " + oContext.TaskExecution.Task.Name
    oContext.LogResult(sReturn)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_SubTask_IVbsTaskExecution.htm`*
