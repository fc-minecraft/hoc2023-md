### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Lunch Time
The automatic food dispensor is missing students it can't detect. Read through the code and update it so it's able to find students of all different heights.

## Step 1


```ghost
    hoc2023.scene1_LunchTime()
    hoc2023.scene1_DetectStudent()
    hoc2023.scene1_ScanHorizontally()
    hoc2023.scene1_SmartScan()
    hoc2023.scene1_ServeLunch()
    hoc2023.scene1_WaitStudent()
```
```template
    while (hoc2023.scene1_LunchTime()) {
        hoc2023.scene1_ScanHorizontally()
        if (hoc2023.scene1_DetectStudent()) {
            hoc2023.scene1_ServeLunch()
        } else {
            hoc2023.scene1_WaitStudent()
        }
    }
```

```package
artemis-ts=github:ReWrite-Media/hoc2023-ts#v0.0.3
```