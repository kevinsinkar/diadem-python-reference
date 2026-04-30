---
title: "Properties (Parallel Process Control)"
---

# Properties

9 properties from `ParallelProcessControl.chm`.

| Name | Summary |
| --- | --- |
| [`ILocalWorker.ID`](ilocalworker-id.md) | Specifies the ID of the LocalWorker object. Use the property to specify the current ID in a worker script. |
| [`ILocalWorker.MasterApplication`](ilocalworker-masterapplication.md) | Specifies which master application started the Worker object. Use the MasterApplication property to request, for example, the value of a global variable such as R1 in the master. Do not use this property, for example, to start a script in the master because the worker waits until the master application answers. |
| [`IParallelProcessControl.OnWorkerStateChange`](iparallelprocesscontrol-onworkerstatechange.md) | Specifies the name of the user command which DIAdem executes when the Worker status changes. Always create a procedure in the master which is called by OnWorkerStateChange and which checks the error status of the Worker object with the error GetErrorFlag method. |
| [`IParallelProcessControl.Workers`](iparallelprocesscontrol-workers.md) | Returns a collection of all Worker objects in parallel processing. |
| [`IWorker.Application`](iworker-application.md) | Specifies in which application the Worker object runs. Use the Application property to, for example, request the value of a global variable, such as R1, in order to check the progress in the worker. The worker does not answer until it is no longer busy. In this time the master does not execute any other commands. Therefore you should only use this property in exceptional cases. |
| [`IWorker.ID`](iworker-id.md) | Returns the ID of the Worker object. Use the ID to request the current ID of a Worker object from the master. |
| [`IWorker.isRunning`](iworker-isrunning.md) | Specifies whether a Worker object is busy. |
| [`IWorkers.Count`](iworkers-count.md) | Returns the number of Worker objects. |
| [`IWorkers.RunningWorkersCount`](iworkers-runningworkerscount.md) | Returns the number of busy Worker objects. Busy Worker objects are objects that are executing a script. |
