---
title: "IParallelProcessControl.OnWorkerStateChange"
description: "Triggers in parallel processing when a worker object changes its status. The event starts the user command that you assigned to the OnWorkerStateChange property"
---

# IParallelProcessControl.OnWorkerStateChange

!!! abstract "Event &middot; `ParallelProcessControl.chm`"
    Event: OnWorkerStateChange for ParallelProcessControl

Triggers in parallel processing when a worker object changes its status. The event starts the user command that you assigned to the OnWorkerStateChange property. The user command must receive two parameters: The first parameter contains the Worker object and the second parameter the status as an integer value when the user command is called. The status is an enumeration with the following selection terms: 0 eWorkerCreated The worker was started. 1 eWorkerScriptStarting The worker starts the execution of the script. 2 eWorkerScriptFinished The worker finishes the execution of the script. 3 eWorkerRemoving The worker is finishing. Refer to Working with Events in DIAdem for more information on events in DIAdem.

## Signature

```python
obj.OnWorkerStateChange
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eWorkerCreated` | 0 | The worker was started. |
| `eWorkerScriptStarting` | 1 | The worker starts the execution of the script. |
| `eWorkerScriptFinished` | 2 | The worker finishes the execution of the script. |
| `eWorkerRemoving` | 3 | The worker is finishing. |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Data.Root.Clear()
DataFileLoad("Example.tdm","TDM","")
ScriptCmdAdd(CurrentScriptPath + "Callback.vbs")
ParallelProcessControl.OnWorkerStateChange = "CheckState"
for i in range(1, dd.Data.Root.ChannelGroups(2).Channels.Count + 1):
    oMyWorker = ParallelProcessControl.Workers.Add(i,true,"")
    MyArgArray(0) = ChannelsToArray("[2]/[" + i + "]")
    MyArgArray(1) = i
    MyArgArray(2) = 50
    oMyWorker.SetArgument(MyArgArray)
    oMyWorker.Run(CurrentScriptPath + "WorkerScript.vbs","CallbackFct")
Do
Pause(0.1)
ParallelProcessControl.Workers.RemoveAll()
```

```python
DBM ("Worker " + LocalWorker.ID)
dd.Data.Root.Clear()
aInputArg = LocalWorker.GetArgument

ArrayToChannels(aInputArg(0), Array("tempChannel"))
oTempChannel = dd.Data.GetChannel("/tempChannel")

RMS(oTempChannel,aInputArg(2))  # Do some analysis

aResults(0) = ChannelsToArray("/tempChannel")
aResults(1) = aInputArg(1)
LocalWorker.SetArgument(aResults)

def RMS(Channel, Width):
    for i in range(1 + Width, Channel.Size - Width + 1):
        Sum = 0
        for j in range(i - Width, i + 1):
            Sum = Sum + Channel(j) * Channel(j)
        Channel(i-Width) = Sqr(Sum/Width)
```

```python
def CallbackFct(oWorker):
    aResults = oWorker.GetArgument
    DBM("Worker ID: " + oWorker.ID + " Result#: " + aResults(1))
    ArrayToChannels(aResults(0),array("[2]/[" + aResults(1) + "]"),true)

def CheckState(oWorker,iState):
    # The following statement is not executed. It is only used for autocompletion.
    if False:
        oWorker = ParallelProcessControl.Workers.Add(i,true,"")

    if oWorker.GetErrorFlag:
        DBM ("Error: " + oWorker.GetErrorText)
        oWorker.ResetError
    # select iState
    # case eWorkerCreated
    DBM ("Status "& oWorker.ID + " Created")
    # case eWorkerScriptStarting
    DBM ("Status "& oWorker.ID + " Starting")
    # case eWorkerScriptFinished
    DBM ("Status "& oWorker.ID + " Finished")
    # case eWorkerRemoving
    DBM ("Status "& oWorker.ID + " Removing")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Parallel File Analysis</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a></p>
</div>
</div>

---

*Source: `ParallelProcessControl/events/ParallelProcessControl_Event_OnWorkerStateChange_IParallelProcessControl.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
