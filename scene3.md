### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
Now that we'd decoded the obfuscated words, we could see that the birds are being instructed to move the trash and drop it. Let's update the code so the birds bring the trash to the dumpster.

#### ~ tutorialhint 
Remove the ``||hoc2023Objectives: move trash||`` and ``||hoc2023Objectives: drop trash||`` with the new blocks we learned. Make sure to add them in the correct order.

```ghost
hoc2023.scene3_SearchForGarbage()
hoc2023.scene3_Garbage()
hoc2023.scene3_PickupGarbage()
hoc2023Objectives.scene3_MoveGarbage()
hoc2023Objectives.scene3_DropGarbage()
hoc2023.scene3_Battery()
hoc2023.scene3_FindUtilityBox()
hoc2023.scene3_StartCharging()
hoc2023.scene3_Charging()
hoc2023.scene3_StopCharging()
hoc2023.scene3_ContinueFlightLoop()
hoc2023Objectives.scene3_TakeToDumpster()
hoc2023Objectives.scene3_RecycleGarbage()
```
```template
while (hoc2023.scene3_SearchForGarbage()) {
    if (hoc2023.scene3_Garbage() == true) {
        hoc2023.scene3_PickupGarbage()
        hoc2023Objectives.scene3_MoveGarbage()
        hoc2023Objectives.scene3_DropGarbage()
    }
    if (hoc2023.scene3_Battery() < 20) {
        hoc2023.scene3_FindUtilityBox()
        hoc2023.scene3_StartCharging()
        while (hoc2023.scene3_Charging()) {
            if (hoc2023.scene3_Battery() > 80) {
                hoc2023.scene3_StopCharging()
            }
        }
    }
    hoc2023.scene3_ContinueFlightLoop()
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.53
```