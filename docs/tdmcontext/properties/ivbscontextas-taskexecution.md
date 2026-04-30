---
title: "IVbsContextAS.TaskExecution"
description: "Returns the TaskExecution <Analysis Automation> object. The TaskExecution <Analysis Automation> object provides information on the task being executed."
---

# IVbsContextAS.TaskExecution

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: TaskExecution for ContextRun <Analysis Automation>

Returns the TaskExecution <Analysis Automation> object. The TaskExecution <Analysis Automation> object provides information on the task being executed.

## Signature

```python
return_value = obj.TaskExecution
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

*Source: `TDMcontext/properties/TDMContext_property_TaskExecution_IVbsContextAS.htm`*
