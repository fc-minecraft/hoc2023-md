### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
We can't quite read the code because some of it is `obfuscated` which means unclear or obscured. Before we could fix the problem we need to decode those words. Let's follow the birds to see if we could figure out what this code is doing.

#### ~ tutorialhint 
No coding is required here. Exit the coding window and follow the birds.


```ghost
hoc2023Disable.scene3_ObSearchForGarbage()
hoc2023Disable.scene3_ObGarbage()
hoc2023Disable.scene3_ObPickupGarbage()
hoc2023Disable.scene3_ObMoveGarbage()
hoc2023Disable.scene3_ObDropGarbage()
hoc2023Disable.scene3_Battery()
hoc2023Disable.scene3_FindUtilityBox()
hoc2023Disable.scene3_StartCharging()
hoc2023Disable.scene3_Charging()
hoc2023Disable.scene3_StopCharging()
hoc2023Disable.scene3_ContinueFlightLoop()
hoc2023Disable.scene3_ObTakeToDumpster()
hoc2023Disable.scene3_ObRecycleGarbage()
```
```template
while (hoc2023Disable.scene3_ObSearchForGarbage()) {
    if (hoc2023Disable.scene3_ObGarbage() == true) {
        hoc2023Disable.scene3_ObPickupGarbage()
        hoc2023Disable.scene3_ObMoveGarbage()
        hoc2023Disable.scene3_ObDropGarbage()
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
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.51
```