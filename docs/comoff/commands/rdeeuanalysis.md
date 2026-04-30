---
title: "RdeEuAnalysis"
description: "Analyzes the emissions from motor vehicles measured on public transport journeys according to European standards."
---

# RdeEuAnalysis

!!! abstract "Command &middot; `ComOff.chm`"
    Command: RdeEuAnalysis

Analyzes the emissions from motor vehicles measured on public transport journeys according to European standards.

## Signature

```python
return_value = dd.RdeEuAnalysis(SelectionVehicleSpeed, SelectionAltitude, SelectionExhaustMassFlowRate)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SelectionVehicleSpeed</td>
<td>Specifies the name of the channel with the speed data.<div id="exp_SelectionVehicleSpeed"><table class="Borderless">
<tr><td width="150"><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr><td>The following settings are possible:<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Value</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Channel Name</strong></td></tr>
<tr><td width="150"><donottranslate><pre>1</pre></donottranslate></td>
<td>"VehicleSpeedGPS"</td></tr>
<tr><td width="150"><donottranslate><pre>2</pre>
</donottranslate>
</td>
<td>"VehicleSpeedECU"</td></tr>
<tr><td width="150"><donottranslate><pre>3</pre>
</donottranslate>
</td>
<td>"VehicleSpeedSensor"</td></tr>
</table>
</td></tr>
</table></div>
</td></tr>
<tr><td width="150">SelectionAltitude</td>
<td>Specifies the name of the channel with the altitude data.<div id="exp_SelectionAltitude"><table class="Borderless">
<tr><td width="150"><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr><td>The following settings are possible:<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Value</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Channel Name</strong></td></tr>
<tr><td width="150"><donottranslate><pre>1</pre></donottranslate></td>
<td>"AltitudeGPS"</td></tr>
<tr><td width="150"><donottranslate><pre>2</pre>
</donottranslate>
</td>
<td>"AltitudeSensor"</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SelectionExhaustMassFlowRate</td>
<td>Specifies the name of the channel with the mass flow data of the exhaust gas.<div id="exp_SelectionExhaustMassFlowRate"><table class="Borderless">
<tr><td width="150"><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr><td>The following settings are possible:<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Value</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Channel Name</strong></td></tr>
<tr><td width="150"><donottranslate><pre>1</pre></donottranslate></td>
<td>"ExhaustMassFlowRateEFM"</td></tr>
<tr><td width="150"><donottranslate><pre>2</pre>
</donottranslate>
</td>
<td>"ExhaustMassFlowRateECU"</td></tr>
<tr><td width="150"><donottranslate><pre>3</pre>
</donottranslate>
</td>
<td>"ExhaustMassFlowRateSensor"</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuVehicleCategory</td>
<td>Specifies the vehicle category according to Annex II of Directive 70/156/EEC, such as <span class="Monospace">M</span>, <span class="Monospace">M1</span>.<div id="exp_RdeEuVehicleCategory">
<table class="Borderless">
<tr><td>RdeEuVehicleCategory, <a href="#" data-unresolved="1">String</a></td></tr>
<tr><td>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelType</td>
<td>Specifies the fuel to use.<div id="exp_RdeEuFuelType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr><td>1 &lt;= RdeEuFuelType &lt;= <a href="../../../varoff/variables/rdeeunooffueltypes/">RdeEuNoOfFuelTypes</a><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelName</td>
<td>Specifies which fuel is used.<div id="exp_RdeEuFuelName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelExhaustGasDensity</td>
<td>Specifies the density of exhaust gas in kilograms per cubic meter.<div id="exp_RdeEuFuelExhaustGasDensity">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelExhaustGasDensity &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelAlpha</td>
<td>Specifies the molar ratio of hydrogen (H/C) in the fuel.<div id="exp_RdeEuFuelAlpha">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= RdeEuFuelAlpha &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelBeta</td>
<td>Specifies the molar ratio of hydrogen (H/C) in the fuel.<div id="exp_RdeEuFuelBeta">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelBeta &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelGamma</td>
<td>Specifies the molar ratio of sulfur (S/C) in the fuel.<div id="exp_RdeEuFuelGamma">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelGamma &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelDelta</td>
<td>Specifies the molar ratio of nitrogen (N/C) in the fuel.<div id="exp_RdeEuFuelDelta">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelDelta &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelEpsilon</td>
<td>Specifies the molar ratio of oxygen (O/C) in the fuel.<div id="exp_RdeEuFuelEpsilon">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelDelta &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelK_CO</td>
<td>Specifies the density ratio of carbon monoxide to the total density of the exhaust gas.<div id="exp_RdeEuFuelK_CO">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelK_CO &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelK_CO2</td>
<td>Specifies the density ratio of carbon dioxide to the total density of the exhaust gas.<div id="exp_RdeEuFuelK_CO2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelK_CO2 &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelK_NOx</td>
<td>Specifies the density ratio of nitrogen to the total density of the exhaust gas.<div id="exp_RdeEuFuelK_NOx">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelK_NOx &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelK_CH4</td>
<td>Specifies the density ratio of methane to the total density of the exhaust gas.<div id="exp_RdeEuFuelK_CH4">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelK_CH4 &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuFuelK_THC</td>
<td>Specifies the density ratio of hydrocarbons to the total density of the exhaust gas.<div id="exp_RdeEuFuelK_THC">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuFuelK_CH4 &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuWLTPCO2ReferenceMass</td>
<td>Specifies the reference value for the mass of carbon dioxide in kilograms.<div id="exp_RdeEuWLTPCO2ReferenceMass">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuWLTPCO2ReferenceMass &lt;= 10.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuWLTPLowSpeed</td>
<td>Specifies the reference point for the phase of the WLTP cycle at very low speed.<div id="exp_RdeEuWLTPLowSpeed">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuWLTPLowSpeed &lt;= 255.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuWLTPHighSpeed</td>
<td>Specifies the reference point for the high-speed phase of the WLTP cycle.<div id="exp_RdeEuWLTPHighSpeed">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuWLTPHighSpeed &lt;= 255.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuWLTPExtraHighSpeed</td>
<td>Specifies the reference point for the phase of the WLTP cycle at very high speed.<div id="exp_RdeEuWLTPExtraHighSpeed">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0 &lt;= RdeEuWLTPExtraHighSpeed &lt;= 255.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RdeEuPropulsionType</td>
<td>Specifies the propulsion type.<div id="exp_RdeEuPropulsionType">
<table class="Borderless">
<tr>
<td>RdeEuPropulsionType, <a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"ICE"</pre></donottranslate></td>
<td>ICE (Internal combustion engine)</td></tr>
<tr><td width="150"><donottranslate><pre>"NOVC-HEV"</pre></donottranslate></td>
<td>NOVC-HEV (Not off-vehicle charging hybrid electric vehicle)</td></tr>
<tr><td width="150"><donottranslate><pre>"OVC-HEV"</pre></donottranslate></td>
<td>OVC-HEV (Off-vehicle charging hybrid electric vehicle)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150"><em>ChnResult</em></td>
<td>Contains the result channels of the analysis. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.<br attr="ext"/>DIAdem stores the results of the analysis in the channel groups <span class="Monospace">RDE_EU_Results</span> and <span class="Monospace">RDE_EU_MAW</span>. DIAdem stores the summary of the results in custom properties of these two channel groups.<br attr="ext"/>DIAdem stores the determined exhaust gas concentrations, exhaust gas mass flows, data on the route and on the various operating modes (idle, cold start, city, country road, motorway) in the channels of the channel group <span class="Monospace">RDE_EU_Results</span> , DIAdem stores results on the exhaust gas parameters, fuel-specific emissions, the masses of the individual pollutants, and information on the test drive in the custom properties.<br attr="ext"/>DIAdem stores the results of the MAW analysis (Moving Average Window) in the channels of the channel group <span class="Monospace">RDE_EU_MAW</span> . DIAdem stores the pollutant emissions and the maximum speeds for the different load types (city, country road, and motorway) in the custom properties,</td>
</tr>
</table>
</div>

---

*Source: `ComOff/RdeEuAnalysis.htm`*
