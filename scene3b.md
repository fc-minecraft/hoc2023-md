### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Проблема с птицами

## Step 1
``||scene5_RedMatchAgent:Здесь код не требуется.|`` Теперь мы заметили, что есть два неиспользованных блока, которые могут быть полезны. Выйди из окна кодирования и посмотри, сможешь ли ты найти мусорный бак, чтобы выбросить туда мусор. ``||scene5_RedMatchAgent:Выйди из окна кодирования и следуй за птицами.||``

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