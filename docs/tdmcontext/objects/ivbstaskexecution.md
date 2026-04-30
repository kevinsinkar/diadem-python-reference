---
title: "IVbsTaskExecution"
description: "The TaskExecution <Analysis Automation> object provides information on the task being executed. The TaskInfo object contains information on the executable task."
---

# IVbsTaskExecution

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: TaskExecution <Analysis Automation>

The TaskExecution <Analysis Automation> object provides information on the task being executed. The TaskInfo object contains information on the executable task. The ProcedureInfo object contains information on the analysis automation procedure of a task.

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
<p><a href="../../properties/ivbstaskexecution-id/">Id</a> | <a href="../../properties/ivbstaskexecution-procedure/">Procedure</a> | <a href="../../properties/ivbstaskexecution-subtask/">SubTask</a> | <a href="../../properties/ivbstaskexecution-task/">Task</a>| <a href="../../properties/ivbstaskexecution-user/">User</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-taskexecution/">TaskExecution</a> | <a href="../ivbscontextasinit/">ContextInitialize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasinit-taskexecution/">TaskExecution</a> | <a href="../ivbscontextas/">ContextRun &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextas-taskexecution/">TaskExecution</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsTaskExecution.htm`*
