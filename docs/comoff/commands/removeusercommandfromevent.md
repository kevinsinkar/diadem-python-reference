---
title: "RemoveUserCommandFromEvent"
description: "Deletes a single user command from a list of user commands which you assigned to an event ."
---

# RemoveUserCommandFromEvent

!!! abstract "Command &middot; `ComOff.chm`"
    Command: RemoveUserCommandFromEvent

Deletes a single user command from a list of user commands which you assigned to an event .

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
#Do something
RemoveUserCommandFromEvent("View.Events.OnActiveSheetChanged","MyFirstCommand")
```

---

*Source: `ComOff/RemoveUserCommandFromEvent.htm`*
