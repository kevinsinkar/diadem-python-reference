---
title: "IVbsTaskInfo"
description: "The TaskInfo <Analysis Automation> object provides information about a task from the list of executable tasks. The TaskExecution object contains information on "
---

# IVbsTaskInfo

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: TaskInfo <Analysis Automation>

The TaskInfo <Analysis Automation> object provides information about a task from the list of executable tasks. The TaskExecution object contains information on the executed task. The ProcedureInfo object contains information on the analysis automation procedure of a task.

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    sReturn = "ID of current task: " + oContext.TaskExecution.Id + "\r\n"
    sReturn = sReturn + "Subtask ID of current task: " + oContext.TaskExecution.SubTask.Id + "\r\n"
    sReturn = sReturn + "Procedure ID of excecutable task in the tasks list: " + oContext.TaskExecution.Procedure.Id + "\r\n"
    sReturn = sReturn + "Procedure name of excecutable task in the tasks list: " + oContext.TaskExecution.Procedure.Name + "\r\n"
    sReturn = sReturn + "Task ID of excecutable task in the tasks list: " + oContext.TaskExecution.Task.Id  + "\r\n"
    sReturn = sReturn + "Task name of excecutable task in the tasks list: " + oContext.TaskExecution.Task.Name
    oContext.LogResult(sReturn)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbstaskinfo-id/">Id</a> | <a href="../../properties/ivbstaskinfo-name/">Name</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbstaskexecution/">TaskExecution &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbstaskexecution-task/">Task</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsTaskInfo.htm`*
