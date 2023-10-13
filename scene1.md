### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Food Dispenser

## Step 1
The automatic food dispensor is missing students it can't detect. Read through the code and update it so it's able to find students of all different heights.

#### ~ tutorialhint 
Set the ``||hoc2023Objectives:scan <type>||`` block to a `smart` scan.


```ghost
    hoc2023.scene1_LunchTime()
    hoc2023.scene1_DetectStudent()
    hoc2023Objectives.scene1_Scan()
    hoc2023.scene1_ServeLunch()
    hoc2023.scene1_WaitStudent()
```
```template
    while (hoc2023.scene1_LunchTime()) {
        hoc2023Objectives.scene1_Scan()
        if (hoc2023.scene1_DetectStudent()) {
            hoc2023.scene1_ServeLunch()
        }
        hoc2023.scene1_WaitStudent()
    }
```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.53
```