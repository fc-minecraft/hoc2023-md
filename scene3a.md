### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
``||scene5_RedMatchAgent:No coding is required here.|`` We can't quite understand the code because some of it is unclear and hidden. Before we could fix the problem we need to decode the secret words. Let's follow the birds to see if we could figure out what this code is doing. ``||scene5_RedMatchAgent:Exit the coding window and follow the birds.||``


```ghost
hoc2023Disable.scene3_ObSearchForGarbage()
hoc2023Disable.scene3_ObGarbage()
hoc2023Disable.scene3_ObPickupGarbage()
hoc2023Disable.scene3_ObMoveGarbage()
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
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```