---
title: "StatsPropertyName"
description: "Specifies the name of the custom properties for the statistical values calculated by the commands ChnStatisticsBlockCalc and ChnStatisticsChannelCalc ."
---

# StatsPropertyName

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: StatsPropertyName

Specifies the name of the custom properties for the statistical values calculated by the commands ChnStatisticsBlockCalc and ChnStatisticsChannelCalc .

## Python example

```python
dd.ChnResult = dd.ChnStatisticsChannelCalc("[1]/[1]", dd.eStatsMinimum + dd.eStatsMaximum + dd.eStatsGeometricMean)
print(dd.StatsPropertyName(dd.eStatsMinimum) , " : " , dd.StatsResult(dd.eStatsMinimum) , "\r\n" , dd.StatsPropertyName(dd.eStatsMaximum) , " : " , dd.StatsResult(dd.eStatsMaximum) , "\r\n" , dd.StatsPropertyName(dd.eStatsGeometricMean) , " : " , dd.StatsResult(dd.eStatsGeometricMean))
```

---

*Source: `VarOff/StatsPropertyName.htm`*
