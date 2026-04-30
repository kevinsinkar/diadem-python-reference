---
title: "ChnStatisticsBlockCalc"
description: "Calculates characteristic statistical values rowwise."
---

# ChnStatisticsBlockCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnStatisticsBlockCalc

Calculates characteristic statistical values rowwise.

## Signature

```python
return_value = dd.ChnStatisticsBlockCalc(ChnList1, StatsSelection, [ StatsStartIndex ], [ StatsEndIndex ], [StatsUsePopulationFormula], [StatsResultChn], [StatsResultChnNames], [StatsResultChnNameFormat])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">StatsSelection</td>
<td>Specifies which statistical characteristic values to calculate.<div id="exp_StatsSelection">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>0 &lt;= StatsSelection &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>The <span class="Monospace">StatsSelection</span> variable can accept the following constants, which you use for calculating several characteristic values with the <span class="Monospace">OR</span> operator:</p>
<table class="Borderless">
<tr>
<td>2^0</td>
<td width="150"><span class="Monospace">eStatsIndex</span></td>
<td>Index number</td>
</tr>
<tr>
<td>2^1</td>
<td width="150"><span class="Monospace">eStatsSum</span></td>
<td>Sum</td>
</tr>
<tr>
<td>2^2</td>
<td width="150"><span class="Monospace">eStatsSumOfSquares</span></td>
<td>Square sum</td>
</tr>
<tr>
<td>2^3</td>
<td width="150"><span class="Monospace">eStatsMinimum</span></td>
<td>Minimum</td>
</tr>
<tr>
<td>2^4</td>
<td width="150"><span class="Monospace">eStatsMaximum</span></td>
<td>Maximum</td>
</tr>
<tr>
<td>2^5</td>
<td width="150"><span class="Monospace">eStatsArithmeticMean</span></td>
<td>Arithmetic mean</td>
</tr>
<tr>
<td>2^6</td>
<td width="150"><span class="Monospace">eStatsSquareMean</span></td>
<td>Root mean square</td>
</tr>
<tr>
<td>2^7</td>
<td width="150"><span class="Monospace">eStatsGeometricMean</span></td>
<td>Geometric mean</td>
</tr>
<tr>
<td>2^8</td>
<td width="150"><span class="Monospace">eStatsHarmonicMean</span></td>
<td>Harmonic mean</td>
</tr>
<tr>
<td>2^9</td>
<td width="150"><span class="Monospace">eStatsLowerQuartile</span></td>
<td>0.25 quantile (lower quartile)</td>
</tr>
<tr>
<td>2^10</td>
<td width="150"><span class="Monospace">eStatsMedian</span></td>
<td>0.50 quantile (median)</td>
</tr>
<tr>
<td>2^11</td>
<td width="150"><span class="Monospace">eStatsUpperQuartile</span></td>
<td>0.75 quantile (upper quartile)</td>
</tr>
<tr>
<td>2^12</td>
<td width="150"><span class="Monospace">eStatsRange</span></td>
<td>Range</td>
</tr>
<tr>
<td>2^13</td>
<td width="150"><span class="Monospace">eStatsStandardDeviation</span></td>
<td>Standard deviation</td>
</tr>
<tr>
<td>2^14</td>
<td width="150"><span class="Monospace">eStatsVariance</span></td>
<td>Variance</td>
</tr>
<tr>
<td>2^15</td>
<td width="150"><span class="Monospace">eStatsVariationCoefficient</span></td>
<td>Variation coefficient</td>
</tr>
<tr>
<td>2^16</td>
<td width="150"><span class="Monospace">eStatsQuartileDistance</span></td>
<td>Quartile distance</td>
</tr>
<tr>
<td>2^17</td>
<td width="150"><span class="Monospace">eStatsRelativeVariationCoefficient</span></td>
<td>Relative variation coefficient</td>
</tr>
<tr>
<td>2^18</td>
<td width="150"><span class="Monospace">eStatsAverageAbsoluteDeviationFromMean</span></td>
<td>Average absolute deviation from mean</td>
</tr>
<tr>
<td>2^19</td>
<td width="150"><span class="Monospace">eStatsAverageAbsoluteDeviationFromMedian</span></td>
<td>Average absolute deviation from median</td>
</tr>
<tr>
<td>2^20</td>
<td width="150"><span class="Monospace">eStatsSkewness</span></td>
<td>Skewness</td>
</tr>
<tr>
<td>2^21</td>
<td width="150"><span class="Monospace">eStatsKurtosis</span></td>
<td>Kurtosis</td>
</tr>
<tr>
<td>2^22</td>
<td width="150"><span class="Monospace">eStatsStandardError</span></td>
<td>Standard error</td>
</tr>
<tr>
<td>2^23</td>
<td width="150"><span class="Monospace">eStatsExcessKurtosis</span></td>
<td>Excess</td>
</tr>
<tr>
<td>2^24</td>
<td width="150"><span class="Monospace">eStatsThreeSigma</span></td>
<td>Three sigma</td>
</tr>
<tr>
<td>2^25</td>
<td width="150"><span class="Monospace">eStatsSixSigma</span></td>
<td>Six sigma</td>
</tr>
<tr>
<td>2^26</td>
<td width="150"><span class="Monospace">eStatsNormDistB</span></td>
<td>Anderson-Darling test</td>
</tr>
<tr>
<td>2^27</td>
<td width="150"><span class="Monospace">eStats0025Quantile</span></td>
<td>0.025 quantile</td>
</tr>
<tr>
<td>2^28</td>
<td width="150"><span class="Monospace">eStats0975Quantile</span></td>
<td>0.975 quantile</td>
</tr>
<tr>
<td>(2^31)-1</td>
<td width="150"><span class="Monospace">eStatsAll</span></td>
<td>All values</td>
</tr>
</table>
<p>In addition, you can use the following constants which contain the associated characteristic values: <span class="Monospace">eStatsGroupAverageAbsDeviation</span>, <span class="Monospace">eStatsGroupDispersion</span>, <span class="Monospace">eStatsGroupExtremeValues</span>, <span class="Monospace">eStatsGroupForm</span>, <span class="Monospace">eStatsGroupMeanValues</span>, <span class="Monospace">eStatsGroupQuantiles</span>, and <span class="Monospace">eStatsGroupSums</span>.</p>
</div></td></tr>
<tr><td width="150">[StatsStartIndex]</td>
<td>Specifies the start row of the channel to be evaluated. The default value is <span class="Monospace">NoValue</span> which means that DIAdem starts from the first row.<div id="exp_StatsStartIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>1 &lt;= StatsStartIndex &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[StatsEndIndex]</td>
<td>Specifies the end row of the channel to be evaluated. The default value is <span class="Monospace">NoValue</span>, which specifies that DIAdem uses the channel length.<div id="exp_StatsEndIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>1 &lt;= StatsEndIndex &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[StatsUsePopulationFormula]</td>
<td>Specifies whether DIAdem calculates the characteristic values based on the population or on the sample. If the value is <span class="Monospace">False</span>, DIAdem calculates the characteristic values based on samples. The default value is <span class="Monospace">False</span>.<div id="exp_StatsUsePopulationFormula">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[StatsResultChn]</td>
<td>Specifies whether DIAdem stores the statistics results in data channels. The default value is <span class="Monospace">False</span>.<div id="exp_StatsResultChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[StatsResultChnNames]</td>
<td>Specifies whether DIAdem stores the input channel names of the descriptive statistics in a text channel. The default value is <span class="Monospace">False</span>.<div id="exp_StatsResultChnNames">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[StatsResultChnNameFormat]</td>
<td>Specifies how DIAdem stores the input channel names of the descriptive statistics in a text channel. The default value is <span class="Monospace">False</span>.<div id="exp_StatsResultChnNameFormat">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"NameName"</pre></donottranslate></td>
<td>Group name/Channel name</td></tr>
<tr><td width="150"><donottranslate><pre>"IndexName"</pre></donottranslate></td>
<td>[Group index]/Channel name</td></tr>
<tr><td width="150"><donottranslate><pre>"NameIndex"</pre></donottranslate></td>
<td>Group name/[Channel index]</td></tr>
<tr><td width="150"><donottranslate><pre>"IndexIndex"</pre></donottranslate></td>
<td>[Group index]/[Channel index]</td></tr>
<tr><td width="150"><donottranslate><pre>"OnlyName"</pre></donottranslate></td>
<td>Only channel name</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or the result channels with the characteristic values. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
MyChannels = dd.Data.GetChannels("[4]/Temperature*")
dd.ChnResult = dd.ChnStatisticsBlockCalc(MyChannels, dd.eStatsMinimum + dd.eStatsMaximum + dd.eStatsArithmeticMean,None ,None ,None ,True)
print(dd.ChnResult.Item(1).Name , ": " , dd.ChnResult.Item(1).Values(1))
```

---

*Source: `ComOff/ChnStatisticsBlockCalc.htm`*
