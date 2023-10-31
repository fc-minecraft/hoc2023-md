### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Food Dispenser

## Step 1
The food dispenser is not finding some students because it can't see them properly. Press the green arrow. Pay attention to how the AI looks for and recognizes students. Then, return to the code and make it fair and inclusive so that it finds students of ALL heights. 

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