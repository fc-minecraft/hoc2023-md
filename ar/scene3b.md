### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
``||scene5_RedMatchAgent:لا يوجد ترميز مطلوب هنا.|`` لقد لاحظنا وجود بلوكين غير مستخدمين قد يكون لهما فائدة.  اخرج من نافذة البرمجة وابحث عن حاوية نفايات لوضع القمامة فيها. ``||scene5_RedMatchAgent:اخرج من نافذة الترميز وابحث عن سلة المهملات.||``

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