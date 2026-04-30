---
title: "IInput"
description: "The Input object provides a calculation input. The Input object is an element of the Inputs collection."
---

# IInput

!!! abstract "Object &middot; `ICalculationSet.chm`"
    Object: Input

The Input object provides a calculation input. The Input object is an element of the Inputs collection.

## Python example

```python
for oMyInput in dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs:
    if oMyInput.IsOutputConnected :
        dd.MsgBoxDisp("Input depending on calculation: " + oMyInput.SourceOutput.Calculation.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iinput-adaptortype/">AdaptorType</a> | <a href="../../properties/iinput-calculation/">Calculation</a> | <a href="../../properties/iinput-name/">Name</a> | <a href="../../properties/iinput-optional/">Optional</a> | <a href="../../properties/iinput-reference/">Reference</a> | <a href="../../properties/iinput-referencetype/">ReferenceType</a> | <a href="../../properties/iinput-sourceoutput/">SourceOutput</a> | <a href="../../properties/iinput-tag/">Tag</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iinput-connectoutput/">ConnectOutput</a> | <a href="../../methods/iinput-disconnectoutput/">DisconnectOutput</a> | <a href="../../methods/iinput-isoutputconnected/">IsOutputConnected</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/inputlist/">InputList</a>.<a href="../../methods/iinputlist-item/">Item</a> | <a href="../../collections/inputs/">Inputs</a>.<a href="../../methods/iinputcollection-add/">Add</a> | <a href="../../collections/inputs/">Inputs</a>.<a href="../../methods/iinputcollection-addbyoutput/">AddByOutput</a> | <a href="../../collections/inputs/">Inputs</a>.<a href="../../methods/iinputcollection-item/">Item</a> | <a href="../ireferenceabstract/">Reference</a>.<a href="../../properties/ireferenceabstract-parent/">Parent</a> | <a href="../ireferencechannel/">ReferenceChannel</a>.<a href="../../properties/ireferencechannel-parent/">Parent</a> | <a href="../ireferencechannelgroupproperty/">ReferenceChannelGroupProperty</a>.<a href="../../properties/ireferencechannelgroupproperty-parent/">Parent</a> | <a href="../ireferencechannellist/">ReferenceChannelList</a>.<a href="../../properties/ireferencechannellist-parent/">Parent</a> | <a href="../ireferencechannelproperty/">ReferenceChannelProperty</a>.<a href="../../properties/ireferencechannelproperty-parent/">Parent</a> | <a href="../ireferencedatasetproperty/">ReferenceDatasetProperty</a>.<a href="../../properties/ireferencedatasetproperty-parent/">Parent</a> | <a href="../ireferencevalue/">ReferenceValue</a>.<a href="../../properties/ireferencevalue-parent/">Parent</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_IInput.htm`*
