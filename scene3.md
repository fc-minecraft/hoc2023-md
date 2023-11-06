### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
Now that we've uncovered the secret words, we can tell that the birds are told to pick up the trash, but there's nowhere to put it. Let's update the code by using different instructions so the birds can handle the trash in a better way, like flying it to the dumpster and dropping it there.

#### ~ tutorialhint 
Remove the ``||hoc2023Objectives: move trash||`` with the two new blocks we learned. Make sure to add them in the correct order.

```ghost
hoc2023.scene3_SearchForGarbage()
hoc2023.scene3_Garbage()
hoc2023.scene3_PickupGarbage()
hoc2023Objectives.scene3_MoveGarbage()
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
    }
    hoc2023.scene3_ContinueFlightLoop()
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```