---
title: "ISystemInfo"
description: "The SystemInfo object provides information about your system."
---

# ISystemInfo

!!! abstract "Object &middot; `SystemInfo.chm`"
    Object: SystemInfo

The SystemInfo object provides information about your system.

## Python example

```python
sOutput =           "No. of CPUs:                   " + "\t" + str(dd.SystemInfo.CPUCount) + "\r\n"
sOutput = sOutput + "Total physical memory:         " + "\t" + str(dd.SystemInfo.PhysicalMemoryTotal) + "\r\n"
sOutput = sOutput + "Available physical memory:     " + "\t" + str(dd.SystemInfo.PhysicalMemoryAvailable) + "\r\n" +"\r\n"
sOutput = sOutput + "Total commit size:             " + "\t" + str(dd.SystemInfo.SystemCommitLimit) + "\r\n"
sOutput = sOutput + "Total used commit size:        " + "\t" + str(dd.SystemInfo.SystemCommitTotal) + "\r\n"
sOutput = sOutput + "Process information:           " + "\r\n"
sOutput = sOutput + "Used physical memory:          " + "\t" + str(dd.SystemInfo.ProcessMemoryUsage) + "\r\n"
sOutput = sOutput + "Maximum virtual size:          " + "\t" + str(dd.SystemInfo.ProcessMaxVirtualSize) + "\r\n"
sOutput = sOutput + "Virtual size:                  " + "\t" + str(dd.SystemInfo.ProcessVirtualSize) + "\r\n"
sOutput = sOutput + "Commit size used by process    " + "\t" + str(dd.SystemInfo.ProcessCommitSize) + "\r\n"
sOutput = sOutput + "No. of GDI objects:            " + "\t" + str(dd.SystemInfo.ProcessGDIObjects) + "\r\n"
sOutput = sOutput + "No. of handles:                " + "\t" + str(dd.SystemInfo.ProcessHandleCount) + "\r\n"
print(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/isysteminfo-cpucount/">CPUCount</a> | <a href="../../properties/isysteminfo-physicalmemoryavailable/">PhysicalMemoryAvailable</a> | <a href="../../properties/isysteminfo-physicalmemorytotal/">PhysicalMemoryTotal</a> | <a href="../../properties/isysteminfo-processcommitsize/">ProcessCommitSize</a> | <a href="../../properties/isysteminfo-processgdiobjects/">ProcessGDIObjects</a> | <a href="../../properties/isysteminfo-processhandlecount/">ProcessHandleCount</a> | <a href="../../properties/isysteminfo-processmaxvirtualsize/">ProcessMaxVirtualSize</a> | <a href="../../properties/isysteminfo-processmemoryusage/">ProcessMemoryUsage</a> | <a href="../../properties/isysteminfo-processvirtualsize/">ProcessVirtualSize</a> | <a href="../../properties/isysteminfo-systemcommitlimit/">SystemCommitLimit</a> | <a href="../../properties/isysteminfo-systemcommittotal/">SystemCommitTotal</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2>
</div>
</div>

---

*Source: `SystemInfo/objects/SystemInfo_Objects_ISystemInfo.htm`*
