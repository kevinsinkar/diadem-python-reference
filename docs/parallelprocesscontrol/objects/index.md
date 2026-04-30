---
title: "Objects (Parallel Process Control)"
---

# Objects

3 objects from `ParallelProcessControl.chm`.

| Name | Summary |
| --- | --- |
| [`ILocalWorker`](ilocalworker.md) | A Worker uses the LocalWorker object to exchange data with the master application. |
| [`IParallelProcessControl`](iparallelprocesscontrol.md) | The ParallelProcessControl object provides parallel processing in DIAdem. The ParallelProcessControl object starts more DIAdem applications which run in the background or in the foreground, or you can request the status of a Worker object . You cannot use the ParallelProcessControl object in Analysis Server scripts. In the OnWorkerStateChange for ParallelProcessControl property, you can define a user command that DIAdem executes when the worker status changes. You need at least two scripts for parallel processing. The master script starts the Worker objects and deletes them, transfers parameters and receives the results. The worker script which the worker executes. In this script you receive parameters or transfer results over the LocalWorker object . In the worker scripts you should not open DAC or REPORT objects over DACObjOpen and GraphObjOpen. Exchange data as an Array between master and worker. Use the commands ChannelsToArray and ArrayToChannels to exchange channel data. If you want to exchange large amounts of data, you can save them in a file. Do not use class or object references because in this case the associated code is executed in the master DIAdem. Use the DBM command to output text in a debug window for the error search. |
| [`IWorker`](iworker.md) | In parallel processing the Worker object provides a single worker which you can access with the master DIAdem. Each Worker object corresponds to a DIAdem application which runs in the background or the foreground and from where the main DIAdem application starts. Use the LocalWorker object to access a worker in the worker. |
