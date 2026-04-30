---
title: "Events (Parallel Process Control)"
---

# Events

2 events from `ParallelProcessControl.chm`.

| Name | Summary |
| --- | --- |
| [`IParallelProcessControl.OnScriptFinished`](iparallelprocesscontrol-onscriptfinished.md) | Triggers in parallel processing when a worker object ends the script started with the Run for Worker method. The event starts the user command that you assigned to the OnScriptFinished parameter of the Run for Worker method. This user command must receive one parameter: The parameter contains the Worker object when the user command is called. Refer to Working with Events in DIAdem for more information on events in DIAdem. |
| [`IParallelProcessControl.OnWorkerStateChange`](iparallelprocesscontrol-onworkerstatechange.md) | Triggers in parallel processing when a worker object changes its status. The event starts the user command that you assigned to the OnWorkerStateChange property. The user command must receive two parameters: The first parameter contains the Worker object and the second parameter the status as an integer value when the user command is called. The status is an enumeration with the following selection terms: 0 eWorkerCreated The worker was started. 1 eWorkerScriptStarting The worker starts the execution of the script. 2 eWorkerScriptFinished The worker finishes the execution of the script. 3 eWorkerRemoving The worker is finishing. Refer to Working with Events in DIAdem for more information on events in DIAdem. |
