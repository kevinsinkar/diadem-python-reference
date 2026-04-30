---
title: "Collections (ICalculationSet)"
---

# Collections

6 collections from `ICalculationSet.chm`.

| Name | Summary |
| --- | --- |
| [`CalculationGroups`](calculationgroups.md) | Collection of all Calculation groups in a calculation set. To access a single calculation group in scripts, either use the Item method or enter the index or the name in parentheses. |
| [`CalculationList`](calculationlist.md) | Calculations collection. If a calculation requires an output from an other calculation as an input, DIAdem first executes the other calculation. DIAdem uses this method to specify the sequence in which calculations are to be executed, and automatically expands the volume of calculations to be executed, if required. This collection is not name oriented so that the collection can contain objects with the same name. Use the Item method or specify the index in parenthesis to access an individual input in this collection in scripts. You cannot change the collection elements. |
| [`Calculations`](calculations.md) | Collection of all Calculations of a calculation group. To access an individual calculation in a script use the Item method or enter the index or the name in parentheses. |
| [`InputList`](inputlist.md) | Collection of all the Inputs that are dependent on an output of a calculation. This collection is not name oriented so that the collection can contain objects with the same name. Use the Item method or specify the index in parenthesis to access an individual input in this collection in scripts. You cannot change the collection elements. |
| [`Inputs`](inputs.md) | Collection of all Inputs of a calculation. To access an individual input in scripts, use the Item method, or enter the index or the name in parentheses. |
| [`Outputs`](outputs.md) | Collection of all Outputs of a calculation. To access an individual output in scripts, use the Item method, or enter the index or the name in parentheses. |
