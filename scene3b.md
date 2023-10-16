### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
You decoded the obfuscated words! We could see there's two unused blocks that might help us. Exit the coding window and see if you could find a dumpster to take the trash to.

#### ~ tutorialhint 
No coding is required here. Exit the coding window and find the dumpster.

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
    if (hoc2023Disable.scene3_Battery() < 20) {
        hoc2023Disable.scene3_FindUtilityBox()
        hoc2023Disable.scene3_StartCharging()
        while (hoc2023Disable.scene3_Charging()) {
            if (hoc2023Disable.scene3_Battery() > 80) {
                hoc2023Disable.scene3_StopCharging()
            }
        }
    }
    hoc2023Disable.scene3_ContinueFlightLoop()
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.54
```