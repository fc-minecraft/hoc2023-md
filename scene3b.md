### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
``||scene5_RedMatchAgent:No coding is required here.|`` Now, we noticed there are two unused blocks that might be useful. Leave the coding screen and see if you can find a dumpster to put the trash into. ``||scene5_RedMatchAgent:Exit the coding window and find the dumpster.||``

```ghost
hoc2023Disable.scene3_SearchForGarbage()
hoc2023Disable.scene3_Garbage()
hoc2023Disable.scene3_PickupGarbage()
hoc2023Disable.scene3_MoveGarbage()
hoc2023Disable.scene3_Battery()
hoc2023Disable.scene3_FindUtilityBox()
hoc2023Disable.scene3_StartCharging()
hoc2023Disable.scene3_Charging()
hoc2023Disable.scene3_StopCharging()
hoc2023Disable.scene3_ContinueFlightLoop()
hoc2023Disable.scene3_TakeToDumpster()
hoc2023Disable.scene3_RecycleGarbage()
```
```template
while (hoc2023Disable.scene3_SearchForGarbage()) {
    if (hoc2023Disable.scene3_Garbage() == true) {
        hoc2023Disable.scene3_PickupGarbage()
        hoc2023Disable.scene3_MoveGarbage()
    }
    hoc2023Disable.scene3_ContinueFlightLoop()
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```