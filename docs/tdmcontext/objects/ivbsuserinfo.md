---
title: "IVbsUserInfo"
description: "The UserInfo <Analysis Automation> object provides information about the user who is searching for data in the current task."
---

# IVbsUserInfo

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: UserInfo <Analysis Automation>

The UserInfo <Analysis Automation> object provides information about the user who is searching for data in the current task.

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    sReturn = "ID of current task: " + oContext.TaskExecution.User.Name + "\r\n"
    sReturn = sReturn + "Name of current user: " + oContext.TaskExecution.User.Name + "\r\n"
    sReturn = sReturn + "Security ID of current user: " + oContext.TaskExecution.SubTask.Id
    oContext.LogResult(sReturn)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbsuserinfo-name/">Name</a> | <a href="../../properties/ivbsuserinfo-sid/">SID</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbstaskexecution/">TaskExecution &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbstaskexecution-user/">User</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsUserInfo.htm`*
