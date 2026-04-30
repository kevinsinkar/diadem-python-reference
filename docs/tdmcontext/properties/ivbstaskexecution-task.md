---
title: "IVbsTaskExecution.Task"
description: "Returns the TaskInfo <Analysis Automation> object in Analysis Automation. The TaskInfo <Analysis Automation> object provides information about a task from the l"
---

# IVbsTaskExecution.Task

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Task for TaskExecution <Analysis Automation>

Returns the TaskInfo <Analysis Automation> object in Analysis Automation. The TaskInfo <Analysis Automation> object provides information about a task from the list of executable tasks.

## Signature

```python
return_value = obj.Task
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

*Source: `TDMcontext/properties/TDMContext_property_Task_IVbsTaskExecution.htm`*
