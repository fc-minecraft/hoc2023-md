### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Food Dispenser

## Step 1
The food dispenser that works by itself is not finding some students because it can't see them properly. Look at the code and make it better so it can find students of different heights. Pay attention to how the AI looks for and recognizes students.

#### ~ tutorialhint 
Try a different setting for the ``||hoc2023Objectives:scan <type>||`` block.


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
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```