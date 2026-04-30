---
title: "IInputCollection.AddByOutput"
description: "Generates an input that is dependent on an output of a calculation and adds this input to the Inputs collection. The properties of the generated input correspon"
---

# IInputCollection.AddByOutput

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: AddByOutput for Inputs

Generates an input that is dependent on an output of a calculation and adds this input to the Inputs collection. The properties of the generated input correspond to the properties of the specified output. You can edit the name of the input afterwards. You cannot change the other properties from the specified output. If the output properties change, the changes influence all dependent inputs. If the name of the specified output already exists in the Inputs or Outputs collection, DIAdem does not generate a new object, it displays an error message. If the dependent input is correct, DIAdem also extends the TargetInputs output property.

## Signature

```python
return_value = obj.AddByOutput(Output)
```

## Python example

```python
oMyOutput = dd.CalculationSet.CalculationGroups("Custom").Calculations(1).Outputs(1)
dd.CalculationSet.CalculationGroups("Custom").Calculations(2).Inputs.AddByOutput(oMyOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_AddByOutput_IInputCollection.htm`*
