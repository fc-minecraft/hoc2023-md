### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Проблема с птицами

## Step 1
Теперь, когда мы раскрыли секретные слова, мы понимаем, что птицам велено подбирать мусор, но некуда его девать. Давай обновим код, используя другие инструкции, чтобы птицы могли лучше справляться с мусором, например, отнести его к мусорному баку и выбросить там.

#### ~ tutorialhint 
Замени "переместить мусор" двумя новыми блоками. Убедись, что они добавлены правильном порядке.

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