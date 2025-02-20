### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Bird Trouble

## Step 1
الآن بعد أن اكتشفنا الشيفرات السرية، يمكننا أن نلاحظ أن الطيور مكلفة بجمع القمامة، لكن لا يوجد مكان لوضعها. لنقوم بتحديث التعليمات في الكود بحيث تتمكن الطيور من التعامل مع القمامة بشكل أفضل، مثل نقلها إلى حاوية النفايات وإسقاطها هناك.

#### ~ tutorialhint 
قم بإزالة البلوك``||hoc2023Objectives: move trash||`` باستخدام البلوكين الجديدين اللذين تعلمناهما. تأكد من إضافتهما بالترتيب الصحيح

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