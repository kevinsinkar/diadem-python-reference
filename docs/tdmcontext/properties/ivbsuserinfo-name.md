---
title: "IVbsUserInfo.Name"
description: "Specifies the name of the user who searches for data in the currently executed task. The name can also be empty."
---

# IVbsUserInfo.Name

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Name for UserInfo <Analysis Automation>

Specifies the name of the user who searches for data in the currently executed task. The name can also be empty.

## Signature

```python
obj.Name
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

*Source: `TDMcontext/properties/TDMContext_property_Name_IVbsUserInfo.htm`*
