---
title: "IVbsSubtaskInfo"
description: "The SubTaskInfo <Analysis Automation> object provides information on the subtask being executed."
---

# IVbsSubtaskInfo

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: SubTaskInfo <Analysis Automation>

The SubTaskInfo <Analysis Automation> object provides information on the subtask being executed.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbssubtaskinfo-id/">Id</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbstaskexecution/">TaskExecution &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbstaskexecution-subtask/">SubTask</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsSubtaskInfo.htm`*
