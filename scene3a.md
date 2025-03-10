### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Проблема с птицами

## Step 1
``||scene5_RedMatchAgent:Здесь код не требуется.|`` Мы не можем до конца понять код, потому что часть его скрыта и неясна. Прежде чем мы сможем исправить проблему, нам нужно расшифровать секретные слова. Давай последуем за птицами, чтобы понять, что делает этот код. ``||scene5_RedMatchAgent:Выйди из окна кодирования и следуй за птицами.||``


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
    hoc2023Disable.scene3_ContinueFlightLoop()
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```