---
title: "IVbsTaskExecution.Procedure"
description: "Returns the ProcedureInfo <Analysis Automation> object in Analysis Automation. The ProcedureInfo <Analysis Automation> object provides information on the task b"
---

# IVbsTaskExecution.Procedure

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Procedure for TaskExecution <Analysis Automation>

Returns the ProcedureInfo <Analysis Automation> object in Analysis Automation. The ProcedureInfo <Analysis Automation> object provides information on the task being executed.

## Signature

```python
return_value = obj.Procedure
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

*Source: `TDMcontext/properties/TDMContext_property_Procedure_IVbsTaskExecution.htm`*
