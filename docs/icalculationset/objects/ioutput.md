---
title: "IOutput"
description: "The Output object provides a calculation output. The Output object is an element of the Outputs collection."
---

# IOutput

!!! abstract "Object &middot; `ICalculationSet.chm`"
    Object: Output

The Output object provides a calculation output. The Output object is an element of the Outputs collection.

## Python example

```python
oMyOutput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs(1)
dd.MsgBoxDisp("No of inputs depending on output: " + oMyOutput.TargetInputs.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ioutput-adaptortype/">AdaptorType</a> | <a href="../../properties/ioutput-calculation/">Calculation</a> | <a href="../../properties/ioutput-name/">Name</a> | <a href="../../properties/ioutput-optional/">Optional</a> | <a href="../../properties/ioutput-reference/">Reference</a> | <a href="../../properties/ioutput-referencetype/">ReferenceType</a> | <a href="../../properties/ioutput-tag/">Tag</a> | <a href="../../properties/ioutput-targetinputs/">TargetInputs</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../iinput/">Input</a>.<a href="../../properties/iinput-sourceoutput/">SourceOutput</a> | <a href="../../collections/outputs/">Outputs</a>.<a href="../../methods/ioutputcollection-add/">Add</a> | <a href="../../collections/outputs/">Outputs</a>.<a href="../../methods/ioutputcollection-item/">Item</a> | <a href="../ireferenceabstract/">Reference</a>.<a href="../../properties/ireferenceabstract-parent/">Parent</a> | <a href="../ireferencechannel/">ReferenceChannel</a>.<a href="../../properties/ireferencechannel-parent/">Parent</a> | <a href="../ireferencechannelgroupproperty/">ReferenceChannelGroupProperty</a>.<a href="../../properties/ireferencechannelgroupproperty-parent/">Parent</a> | <a href="../ireferencechannellist/">ReferenceChannelList</a>.<a href="../../properties/ireferencechannellist-parent/">Parent</a> | <a href="../ireferencechannelproperty/">ReferenceChannelProperty</a>.<a href="../../properties/ireferencechannelproperty-parent/">Parent</a> | <a href="../ireferencedatasetproperty/">ReferenceDatasetProperty</a>.<a href="../../properties/ireferencedatasetproperty-parent/">Parent</a> | <a href="../ireferencevalue/">ReferenceValue</a>.<a href="../../properties/ireferencevalue-parent/">Parent</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_IOutput.htm`*
