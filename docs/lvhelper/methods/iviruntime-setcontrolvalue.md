---
title: "IVIRuntime.SetControlValue"
description: "Specifies the value of an input. Depending on the input you forward the value as a single value or as a matrix."
---

# IVIRuntime.SetControlValue

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: SetControlValue for VIRuntime

Specifies the value of an input. Depending on the input you forward the value as a single value or as a matrix.

## Signature

```python
bSetControlValue = Object.SetControlValue(InputName, Value)
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.loadvi(dd.AutoActPath + "Test")
objVI.SetControlValue("Input1", "InputValue")
objVI.run(True)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.loadvi(dd.AutoActPath + "Test")
for I in range( 0, 3+1):
    for J in range( 0, 1+1):
        MyMatrix = []
MyMatrix.append(I + " Row " + j + " column")
objVI.SetControlValue("MyStringVector", MyMatrix)
objVI.run(True)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.loadvi(dd.AutoActPath + "Test")

MyClusterValue = []
MyClusterValue.append(5)#Set Integer in Cluster
for I in range( 0, 3+1):
    for J in range( 0, 1+1):
        MyStringMatrix = []
MyStringMatrix.append(I + " Row " + j + " column")
MyClusterValue = []
MyClusterValue.append(MyStringMatrix)#Set Matrix in Cluster

objVI.SetControlValue("MyCluster", MyClusterValue)
objVI.run(True)
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

*Source: `LVHelper/methods/LVHelper_method_SetControlValue_IVIRuntime.htm`*
