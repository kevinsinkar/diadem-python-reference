---
title: "Methods (Parallel Process Control)"
---

# Methods

13 methods from `ParallelProcessControl.chm`.

| Name | Summary |
| --- | --- |
| [`ILocalWorker.GetArgument`](ilocalworker-getargument.md) | Returns the transfer parameter of the LocalWorker object which you transferred with SetArgument for Worker in the master DIAdem. Exchange data as an Array between master and worker. Use the commands ChannelsToArray and ArrayToChannels to exchange channel data. If you want to exchange large amounts of data, you can save them in a file. Do not use class or object references because in that case the associated code is executed in the master. |
| [`ILocalWorker.SetArgument`](ilocalworker-setargument.md) | Sets the transfer parameter of the LocalWorker object which you can read in the master with GetArgument for Worker . Exchange data as an Array between master and worker. Use the commands ChannelsToArray and ArrayToChannels to exchange channel data. If you want to exchange large amounts of data, you can save them in a file. Do not use class or object references because in that case the associated code is executed in the master. |
| [`IWorker.AbortScript`](iworker-abortscript.md) | Ends a script in a Worker object. The Worker object is not closed. |
| [`IWorker.GetArgument`](iworker-getargument.md) | Returns the transfer parameter of the Worker object which you transferred with SetArgument for LocalWorker in the worker. Exchange data as an Array between master and worker. Use the commands ChannelsToArray and ArrayToChannels to exchange channel data. If you want to exchange large amounts of data, you can save them in a file. Do not use class or object references because in this case the associated code is executed in the master. |
| [`IWorker.GetErrorFlag`](iworker-geterrorflag.md) | Specifies the error status of the Worker object. Always create a procedure in the master which is called by OnWorkerStateChange for ParallelProcessControl and checks the error status of the Worker object. |
| [`IWorker.GetErrorText`](iworker-geterrortext.md) | Specifies the error text of the Worker object. Always create a procedure in the master which is called by OnWorkerStateChange for ParallelProcessControl and which checks the error text of the Worker object. |
| [`IWorker.ResetError`](iworker-reseterror.md) | Resets the error status of the Worker object. Always create a procedure in the master which is called by OnWorkerStateChange for ParallelProcessControl and checks the error status of the Worker object. |
| [`IWorker.Run`](iworker-run.md) | Starts a script in the Worker object. After the worker has finished the script, it executes the command specified in OnScriptFinished . This command executes further actions in the master when the worker has completed its tasks. DIAdem executes this method asynchronously, which means that the program is continued immediately, while the Worker object executes the specified script in a proprietary application. |
| [`IWorker.SetArgument`](iworker-setargument.md) | Sets the transfer parameter of the Worker object which you can read in the worker with GetArgument for LocalWorker . Exchange data as an Array between master and worker. Use the commands ChannelsToArray and ArrayToChannels to exchange channel data. If you want to exchange large amounts of data, you can save them in a file. Do not use class or object references because in that case the associated code is executed in the master. |
| [`IWorkers.Add`](iworkers-add.md) | Launches a DIAdem application as Worker object. To speed up the launching of the Worker object and to minimize the use of resources, launch the Headless Worker object. This hides the application and no files are loaded. You can create a maximum of five worker objects. |
| [`IWorkers.Item`](iworkers-item.md) | Returns the Worker object of a specific ID. |
| [`IWorkers.Remove`](iworkers-remove.md) | Deletes a Worker object and finishes the associated application. As soon as you exit the master, DIAdem automatically closes all previously started workers. |
| [`IWorkers.RemoveAll`](iworkers-removeall.md) | Deletes all Worker objects and closes the associated applications. As soon as you exit the master, DIAdem automatically closes all previously started workers. |
