---
title: "StatsResult"
description: "Specifies the values of the custom properties for the statistical values calculated by the commands ChnStatisticsBlockCalc and ChnStatisticsChannelCalc ."
---

# StatsResult

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: StatsResult

Specifies the values of the custom properties for the statistical values calculated by the commands ChnStatisticsBlockCalc and ChnStatisticsChannelCalc .

## Python example

```python
dd.ChnResult = dd.ChnStatisticsChannelCalc("[1]/[1]", dd.eStatsMinimum + dd.eStatsMaximum + dd.eStatsGeometricMean)
print(dd.StatsPropertyName(dd.eStatsMinimum) , " : " , dd.StatsResult(dd.eStatsMinimum) , "\r\n" , dd.StatsPropertyName(dd.eStatsMaximum) , " : " , dd.StatsResult(dd.eStatsMaximum) , "\r\n" , dd.StatsPropertyName(dd.eStatsGeometricMean) , " : " , dd.StatsResult(dd.eStatsGeometricMean))
```

---

*Source: `VarOff/StatsResult.htm`*
