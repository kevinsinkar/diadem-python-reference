---
title: "INavigator.LoadChannelsByName"
description: "Loads or calculates channels from a channel group of a TDM file or a measurement of an ASAM data store into the Data Portal. If the names given in the Measureme"
---

# INavigator.LoadChannelsByName

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: LoadChannelsByName for Navigator

Loads or calculates channels from a channel group of a TDM file or a measurement of an ASAM data store into the Data Portal. If the names given in the MeasurementQuantityNameList parameter exist, DIAdem loads the respective channels. If the MeasurementQuantityNameList parameter contains the name of a channel that does not exist, the method searches for a calculation with this reference name in the loaded calculation template and executes the calculation. DIAdem saves the loaded and calculated channels in a new channel group in the Data Portal.

## Signature

```python
return_value = obj.LoadChannelsByName(Measurement, MeasurementQuantityNameList, [ImportSettings])
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Object</em></td><td><a href="../../objects/inavigator/">Navigator</a><br attr="ext"/>Object with this method</td></tr>
<tr><td width="150"><em>Measurement</em></td><td>Variant<br attr="ext"/>Specifies the object containing the channel group or the measurement from which the method loads or calculates the channels or measured values given in the <span class="Monospace">MeasurementQuantityNameList</span> parameter.</td></tr>
<tr><td width="150"><em>MeasurementQuantityNameList</em></td><td>Variant<br attr="ext"/>Specifies the array with the list of names for the measurements or channels which the loading process accesses. Use the function <a href="#" data-unresolved="1">Array</a> to specify the list of measured values or channels or the output references of calculations, for example <span class="Monospace">Array("Revs","Torque","Power")</span>.<br attr="ext"/>The following cases are possible:<br attr="ext"/><br attr="ext"/>1) If the given measured value or the given channel exists in the measurement or in the channel group specified in the <span class="Monospace">Measurement</span> parameter, the <span class="Monospace">LoadChannelsByName</span> method loads the given measured values or channels into a new channel group of the Data Portal.<br attr="ext"/><br attr="ext"/>2) If the given measured value or the given channel exists in the measurement or in the channel group specified in the <span class="Monospace">Measurement</span> the <a href="#" data-unresolved="1">Calculation Template</a>, executes the calculation and generates the associated result channel in the new channel group of the Data Portal. If you want to calculate with DIAdem, the calculation must fulfill the following requirements:<ul><li>The name of the output reference of the calculation must be the same as the name given in the <em>MeasurementQuantityNameList</em> parameter, and it must be defined as a channel in the calculation. You can find the name of the output reference in the <strong>Calculation Manager - Edit Calculation</strong> dialog box in the <strong>Reference</strong> column of the <strong>Outputs</strong> area.</li>
<li>Each reference of the input and output channels must refer to the default group and must be entered in the form <span class="Monospace"><em>/ChannelName</em></span>. <span class="Monospace"><em>ChannelName</em></span> corresponds to a channel name.</li>
<li>If several calculations with the name of the output reference given in the <em>MeasurementQuantityNameList</em> parameter in a calculation template exist, DIAdem executes all calculations and adjusts the names to the result channels in the Data Portal according to the <a href="#" data-unresolved="1">Name Conventions</a> in DIAdem.</li></ul><table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If a channel listed in the <em>MeasurementQuantityNameList</em> parameter does not exist and DIAdem does not find a calculation with this output reference, DIAdem ignores this channel or this calculation.</td></tr></table></td></tr>
<tr><td width="150"><em>[ImportSettings]</em></td><td>Variant<br attr="ext"/>Specifies the <a href="#" data-unresolved="1">Loading configuration</a> as object. You can only use a loading configuration if you load data from data stores. If you assign the value <span class="Monospace">Nothing</span> to the <span class="Monospace">ImportSettings</span> parameter, DIAdem creates the standard browse setting for the open data store (Test/SubTest - Measurement - MeasurementQuantity), generates a minimum loading configuration, and then only transfers the name, the unit, and the description of each element into the Data Portal. If you do not assign any value to the <span class="Monospace">ImportSettings</span> parameter, DIAdem uses the loading configuration of the current data store.</td></tr>
<tr><td width="150"><em>oElementList</em></td><td><a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a><br attr="ext"/>Returned object</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If a channel listed in the <em>MeasurementQuantityNameList</em> parameter does not exist and DIAdem does not find a calculation with this output reference, DIAdem ignores this channel or this calculation.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you have selected the inheritance of properties in the <a href="#" data-unresolved="1">DIAdem NAVIGATOR Settings</a> dialog box, the <span class="Monospace">LoadChannelsByName</span> method always passes on the properties to the loaded channels, irrespective of the selected setting.</td></tr></table>
</div>

## Python example

```python
#Creating search
oMyQueryForm = dd.Navigator.Display.CurrDataFinder.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm

#Searching for channel groups
oMyQueryForm.ReturnType = dd.eSearchChannelGroup
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchChannelGroup,"name","=","r*")

#Executing search
oMyQueryForm.Search()

#First channel group of results list
oChnGrp = dd.Navigator.Display.CurrDataFinder.ResultsList.Elements(1)

#Loading calculation set. The calculation must have the reference output name "Calculation"
dd.CalculationSet.Load("MyCalculationSet.tca")
oChnList = dd.Navigator.LoadChannelsByName(oChnGrp, ["Channel1","Channel2","Channel3","Calculation"])
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_LoadChannelsByName_INavigator.htm`*
