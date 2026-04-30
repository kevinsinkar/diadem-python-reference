---
title: "IVIRuntime"
description: "The VIRuntime object enables you to access LabVIEW VIs from DIAdem. Use the VIRuntime object to access VI properties such as the name or the list of terminals. "
---

# IVIRuntime

!!! abstract "Object &middot; `LVHelper.chm`"
    Object: VIRuntime

The VIRuntime object enables you to access LabVIEW VIs from DIAdem. Use the VIRuntime object to access VI properties such as the name or the list of terminals. You also set values of the VIs or execute VIs.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  If you create VIs with LabVIEW and you want these VIs to run only with the LabVIEW Runtime Engine, you must create a source distribution of the VIs. Refer to the LabVIEW help under the search term <strong>Source Distribution</strong> for further information.<p>If LabVIEW cannot interpret relative path specifications in a normal installation, because, for example, you are using Express VIs, you must edit the <span class="Monospace">DIAdem.ini</span> file in the DIAdem program folder. If the file does not exist, you must create this file. Insert the following entry into the <span class="Monospace">DIAdem.ini</span> file:</p>
<pre><donottranslate>[LVRT]
libdir="<em>LabVIEW_ProgramPath</em>"</donottranslate></pre>
<p>The <span class="Monospace">LabVIEW_ProgramPath</span> specifies the LabVIEW program path, for example, <span class="Monospace">C:\Program Files\National Instruments\LabVIEW 8.2</span>.</p><p>After you make this modification, you must restart DIAdem.</p></td>
</tr>
</table>
</div>

## Python example

```python
# Initialize the LVRuntime
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)

# Load "Test.vi"
objVIVIT = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test")

# Call the VI
objVI.Run(True)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

## Members

<div markdown="1">
<div class="Properties"><div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iviruntime-description/">Description</a> | <a href="../../properties/iviruntime-helppath/">HelpPath</a> | <a href="../../properties/iviruntime-helptag/">HelpTag</a> | <a href="../../properties/iviruntime-name/">Name</a> | <a href="../../properties/iviruntime-terminals/">Terminals</a> | <a href="../../properties/iviruntime-version/">Version</a></p>
</div>
</div>
<div class="Methods"><div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iviruntime-getcontrolvalue/">GetControlValue</a> | <a href="../../methods/iviruntime-getcontrolvariant/">GetControlVariant</a> | <a href="../../methods/iviruntime-run/">Run</a> | <a href="../../methods/iviruntime-setcontrolvalue/">SetControlValue</a></p>
</div>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/objects/LVHelper_Objects_IVIRuntime.htm`*
