---
title: "ILocalWorker"
description: "A Worker uses the LocalWorker object to exchange data with the master application."
---

# ILocalWorker

!!! abstract "Object &middot; `ParallelProcessControl.chm`"
    Object: LocalWorker

A Worker uses the LocalWorker object to exchange data with the master application.

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

RMS(oTempChannel,aInputArg(2))  ' Do some analysis

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ilocalworker-id/">ID</a> | <a href="../../properties/ilocalworker-masterapplication/">MasterApplication</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ilocalworker-getargument/">GetArgument</a> | <a href="../../methods/ilocalworker-setargument/">SetArgument</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="./">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ParallelProcessControl/objects/ParallelProcessControl_Objects_ILocalWorker.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
