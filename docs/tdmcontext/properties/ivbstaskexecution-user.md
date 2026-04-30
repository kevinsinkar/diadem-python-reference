---
title: "IVbsTaskExecution.User"
description: "Returns the UserInfo <Analysis Automation> object in Analysis Automation. The UserInfo <Analysis Automation> object provides information about the user who is s"
---

# IVbsTaskExecution.User

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: User for TaskExecution <Analysis Automation>

Returns the UserInfo <Analysis Automation> object in Analysis Automation. The UserInfo <Analysis Automation> object provides information about the user who is searching for data in the task being executed.

## Signature

```python
return_value = obj.User
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    sReturn = "ID of current task: " + oContext.TaskExecution.User.Name + "\r\n"
    sReturn = sReturn + "Name of current user: " + oContext.TaskExecution.User.Name + "\r\n"
    sReturn = sReturn + "Security ID of current user: " + oContext.TaskExecution.SubTask.Id
    oContext.LogResult(sReturn)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_User_IVbsTaskExecution.htm`*
