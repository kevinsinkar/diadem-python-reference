---
title: "SPCProcessCapab"
description: "Calculates the mean, the sigma, and the capability indices of a process."
---

# SPCProcessCapab

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SPCProcessCapab

Calculates the mean, the sigma, and the capability indices of a process.

## Signature

```python
dd.SPCProcessCapab(ChnList, SPCUSL, SPCLSL, SPCSigmaType, SPCSigmaMult, SPCMovingRangeNo, SPCSigmaTol)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Additionally DIAdem saves the calculation results in the following custom properties of the result channel: <span class="Monospace">Result~SPC~ProcessMean, Result~SPC~ProcessSigma, Result~SPC~Limits~UpperNPL</span>, <span class="Monospace">Result~SPC~Limits~LowerNPL</span>, <span class="Monospace">Result~SPC~CapabilityIndexes~CpU</span>, <span class="Monospace">Result~SPC~CapabilityIndexes~CpL</span>, <span class="Monospace">Result~SPC~CapabilityIndexes~Cp</span>, <span class="Monospace">Result~SPC~CapabilityIndexes~Cpk</span>, <span class="Monospace">Result~SPC~NonconformingParts~FracNConf</span>, <span class="Monospace">Result~SPC~NonconformingParts~UpperFracNConf</span>, and <span class="Monospace">Result~SPC~NonconformingParts~LowerFracNConfResultSPCCp</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">SPCUSL</td>
<td>Specifies the upper specification limit of a process.<div id="exp_SPCUSL">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SPCLSL</td>
<td>Specifies the lower specification limit of a process.<div id="exp_SPCLSL">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SPCSigmaType</td>
<td>Specifies which method to use for calculating the process sigma.<div id="exp_SPCSigmaType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"From Range"</pre></donottranslate></td>
<td>Based on mean sample range</td></tr>
<tr><td width="150"><donottranslate><pre>"From StdDev"</pre></donottranslate></td>
<td>Based on mean sample standard deviation</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SPCSigmaMult</td>
<td>Specifies the sigma multiplier for calculating the upper and the lower natural process limits.<div id="exp_SPCSigmaMult">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SPCSigmaMult &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SPCMovingRangeNo</td>
<td>Specifies the number of samples that are to be included in the moving range if the sample size is 1, which means the channels with length 1.<div id="exp_SPCMovingRangeNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>2 &lt;= SPCMovingRangeNo &lt;= 25</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SPCSigmaTol</td>
<td>Specifies the sigma multiplier for calculating the process capability index.<div id="exp_SPCSigmaTol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SPCSigmaTol &lt;= 1E300</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td width="150">SPCProcessMean</td><td>Receives the mean value of a process.<div id="exp_SPCProcessMean">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="47" src="image/f_SPCProcessmean.gif" width="211"/></p>
</div></td></tr>
<tr>
<td width="150">SPCProcessSigma</td><td>Receives the standard deviation (sigma) of a process.<div id="exp_SPCProcessSigma">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="140" src="image/f_SPCProcessSigma.gif" width="405"/></p>
<table class="Borderless">
<tr>
<td width="150"><span style="text-decoration: overline"><em><span class="Monospace">σ</span></em></span></td><td>Specifies the average sample standard deviation.</td>
</tr>
<tr>
<td width="150"><span style="text-decoration: overline"><em><span class="Monospace">R</span></em></span></td><td>Specifies the average sample range.</td>
</tr>
<tr>
<td width="150"><em><span class="Monospace">m<span style="text-decoration: overline">R</span></span></em></td><td>Specifies the average moving range.</td>
</tr>
<tr><td width="150"><em><span class="Monospace">c<sub>4 </sub>, d<sub>2</sub></span></em></td><td>Specifies a factor in relation to the sample size N.</td></tr></table>
</div></td></tr>
<tr>
<td width="150">SPCUpperNPL</td><td>Receives the upper natural process limit of a process.<div id="exp_SPCUpperNPL">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="20" src="image/f_SPCUpperNPL.gif" width="483"/></p>
</div></td></tr>
<tr>
<td width="150">SPCLowerNPL</td><td>Receives the lower natural process limit of a process.<div id="exp_SPCLowerNPL">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="20" src="image/f_SPCLowerNPL.gif" width="484"/></p>
</div></td></tr>
<tr>
<td width="150">SPCCpU</td><td>Receives the one-sided upper process capability index C<sub>pU</sub>.<div id="exp_SPCCpU">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="41" src="image/f_SPCCPU.gif" width="306"/></p>
</div></td></tr>
<tr>
<td width="150">SPCCpL</td><td>Receives the one-sided lower process capability index C<sub>pL</sub>.<div id="exp_SPCCpL">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="41" src="image/f_SPCCPL.gif" width="303"/></p>
</div></td></tr>
<tr>
<td width="150">SPCCp</td><td>Receives the process capability index C<sub>p</sub>.<div id="exp_SPCCp">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="41" src="image/f_SPCCP.gif" width="267"/></p>
</div></td></tr>
<tr>
<td width="150">SPCCpk</td><td>Receives the process capability index C<sub>pk</sub>.<div id="exp_SPCCpk">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
<p><img height="23" src="image/f_SPCCPk.gif" width="142"/></p>
</div></td></tr>
<tr>
<td width="150">SPCFracNConf</td><td>Receives the estimated fraction nonconforming in ppm based on a normal process distribution<div id="exp_SPCFracNConf">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
</div></td></tr>
<tr>
<td width="150">SPCUFracNConf</td><td>Receives the estimated fraction nonconforming in ppm above the upper spec limit based on a normal process distribution.<div id="exp_SPCUFracNConf">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
</div></td></tr>
<tr>
<td width="150">SPCLFracNConf</td><td>Receives the estimated fraction nonconforming in ppm below the lower spec limit based on a normal process distribution.<div id="exp_SPCLFracNConf">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("Grp/Sample*")
dd.SPCProcessCapab(oMyChannelList, 5.2, 4.8, "From StdDev", 3, 2, 6)
```

---

*Source: `ComOff/SPCProcessCapab.htm`*
