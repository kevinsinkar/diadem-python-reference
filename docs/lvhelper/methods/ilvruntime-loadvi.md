---
title: "ILVRuntime.LoadVI"
description: "Loads a VI."
---

# ILVRuntime.LoadVI

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: LoadVI for LVRuntime

Loads a VI.

## Signature

```python
return_value = obj.LoadVI(VIPath)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  If you create VIs with LabVIEW and you want these VIs to run only with the LabVIEW Runtime Engine, you must create a source distribution of the VIs. Refer to the LabVIEW help under the search term <strong>Source Distribution</strong> for further information.<p>If LabVIEW cannot interpret relative path specifications in a normal installation, because, for example, you are using Express VIs, you must edit the <span class="Monospace">DIAdem.ini</span> file in the DIAdem program folder. If the file does not exist, you must create this file. Insert the following entry into the <span class="Monospace">DIAdem.ini</span> file:</p>
<pre><donottranslate>[LVRT]
libdir="<em><donottranslate>LabVIEW_ProgramPath</donottranslate></em>"</donottranslate></pre>
<p>The <span class="Monospace">LabVIEW_ProgramPath</span> specifies the LabVIEW program path, such as <span class="Monospace">C:\Program Files\National Instruments\LabVIEW 8.2</span>.</p><p>After you make this modification, you must restart DIAdem.</p></td></tr></table>
</div>

## Python example

```python
# Initialize the LVRuntime
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)

# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test")

# Call the VI
objVI.Run(True)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/methods/LVHelper_method_LoadVI_ILVRuntime.htm`*
