---
title: "AddUserCommandToEvent"
description: "Adds a user command to a list of user commands which you assign to an event . If you execute the AddUserCommandToEvent command several times, you can assign sev"
---

# AddUserCommandToEvent

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AddUserCommandToEvent

Adds a user command to a list of user commands which you assign to an event . If you execute the AddUserCommandToEvent command several times, you can assign several user commands to the same event.

## Parameters

<div markdown="1">
<table class="Borderless"><tr>
<td width="150"><em>EventName</em></td><td>String<br attr="ext"/>Specifies the name of a DIAdem event. You cannot transfer the event as a reference ("by reference").</td></tr><tr>
<td width="150"><em>UserCommandName</em></td><td>String<br attr="ext"/>Specifies a user command registered in DIAdem.</td></tr></table>
</div>

## Python example

```python
dd.AddUserCommandToEvent("View.Events.OnActiveSheetChanged","MyFirstCommand")
dd.AddUserCommandToEvent("View.Events.OnActiveSheetChanged","MySecondCommand")
```

---

*Source: `ComOff/AddUserCommandToEvent.htm`*
