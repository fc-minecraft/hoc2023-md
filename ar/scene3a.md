### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
``||scene5_RedMatchAgent:لا يوجد ترميز مطلوب هنا.|`` لا يمكننا فهم الشيفرة بشكل كامل لأن بعض أجزائها غير واضحة ومخفية. قبل أن نتمكن من حل المشكلة، نحتاج إلى فك رموز الشفرات السرية. لنتبع الطيور لنرى إذا كان بإمكاننا اكتشاف ما تفعله هذه الشيفرة. ``||scene5_RedMatchAgent:اخرج من نافذة الترميز واتبع الطيور.||``


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