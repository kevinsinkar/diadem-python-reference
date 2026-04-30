---
title: "IRepCustomScalingAxisSystem2DContextInt.CustomScalingID"
description: "Specifies the ID of a user-defined axis scaling in a 2D axis system in DIAdem REPORT. Use the CustomScalingID property, for example, if you want to scale severa"
---

# IRepCustomScalingAxisSystem2DContextInt.CustomScalingID

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CustomScalingID for CustomScalingAxisSystem2DContext

Specifies the ID of a user-defined axis scaling in a 2D axis system in DIAdem REPORT. Use the CustomScalingID property, for example, if you want to scale several axes differently and do not want to define an individual event for each scaling. You can define all axes scalings in one event and assign the associated axes through the CustomScalingID property.

## Signature

```python
obj.CustomScalingID
```

## Python example

```python
def MyCustomScalingEvent2D(Context):
    if Context.CustomScalingID == "MotorWarm" :
        pass # Implement your scaling code here
    elif Context.CustomScalingID == "MotorCold" :
        pass # Implement your scaling code here
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CustomScalingID_IRepCustomScalingAxisSystem2DContextInt.htm`*
