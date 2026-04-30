---
title: "ISystemInfo.ProcessHandleCount"
description: "Returns the number of handles used by the process."
---

# ISystemInfo.ProcessHandleCount

!!! abstract "Property &middot; `SystemInfo.chm`"
    Property: ProcessHandleCount for SystemInfo

Returns the number of handles used by the process.

## Signature

```python
obj.ProcessHandleCount
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="../../objects/isysteminfo/">Objects Overview</a></p>
</div>
</div>

---

*Source: `SystemInfo/properties/SystemInfo_property_ProcessHandleCount_ISystemInfo.htm`*
