---
title: "ChnStatisticsMovingWindowAsymmetric"
description: "Calculates statistical characteristic values channel by channel, whereby the characteristic values are calculated through an asymmetrical window that is moved a"
---

# ChnStatisticsMovingWindowAsymmetric

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnStatisticsMovingWindowAsymmetric

Calculates statistical characteristic values channel by channel, whereby the characteristic values are calculated through an asymmetrical window that is moved across the channel values. You can separately specify the window size before and after the current channel value. If there are not enough elements at the endpoints, DIAdem will automatically cut off the window.

## Signature

```python
return_value = dd.ChnStatisticsMovingWindowAsymmetric( Y , StatsSelection, WidthBefore , WidthAfter , [StatsUsePopulationFormula])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel for which you want to calculate statistical characteristic values.</td></tr>
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
<td>Minimum value</td>
</tr>
<tr>
<td>2^4</td>
<td width="150"><span class="Monospace">eStatsMaximum</span></td>
<td>Maximum value</td>
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
<tr><td width="150">WidthBefore</td>
<td>Specifies the window width before the current channel value.<div id="exp_WidthBefore">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>0 &lt;= WidthBefore &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">WidthAfter</td>
<td>Specifies the window width after the current channel value.<div id="exp_WidthAfter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>0 &lt;= WidthAfter &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
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
dd.ChnResult = dd.ChnStatisticsMovingWindowAsymmetric("[1]/[1]", dd.eStatsMinimum + dd.eStatsMaximum + dd.eStatsGeometricMean, 2, 5)
```

---

*Source: `ComOff/ChnStatisticsMovingWindowAsymmetric.htm`*
